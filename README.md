# DNS blocking lists, Pihole, Unbound for cname-cloacking, trackers or intrusive advertising.


## Why ?

Cname-cloacking is in breach of European law (GDPR) and the law in many countries (California and Australia seem well inspired too) because they hide the DNS references of the site you are visiting. It is therefore impossible to obtain user consent for these third-party sites and the immediate effect is that you are tracked on all sorts of sites.

This is a more pernicious method than third-party cookies because it is tacit and there is no recourse. It's a real goldmine for the companies that use it.
It's staggering when you consider that some of these companies boast that they can be connected to 600 other trackers.

They can keep your data for as long as they like, since it does not officially exist. This can mean your whole life, as we have seen with databases revealed that have 2 or 3 times the number of people on earth.

Would you like to have a spy on your shoulder from morning to night, analysing your every move throughout the day, right down to the brand of toilet paper you use?

A recent revelation showed that certain viruses could hide in the advertisements of a major global company using information that was not available to the public. This is nothing new, but now it's been proven.

The issue of energy savings and the autonomy of our connected devices is now very important. It's a question of ecological common sense. 
Premature ageing due to over-solicitation of advertising is a major factor. The image of a vehicle in overdrive dragging advertising hoardings seems appropriate to me.


## About this data

The data in these lists is public and accessible to anyone capable of using a DNS query tool such as nslookup, dig, drill or whois, etc. and their graphical equivalents.

Some web pages will go from 10 mb to 1 mb! (<https://www.laquadrature.net/2020/10/05/le-deguisement-des-trackers-par-cname/>). 
 
The bandwidth saved results in energy savings at all levels of the Internet from servers to hubs, right down to our devices.


## Unbound for Linux, Mac and Windows

You can install the excellent DNS software that also caches DNS unbound: https://www.nlnetlabs.nl/projects/unbound/about/
You can then include the stub-zone list [stub-zone](https://github.com/Vincent-Millane/cname-cloaking/blob/main/stub-zone).


## Pihole for Linux, Mac and Windows

For a family or with the multitude of connected objects, installing Pi-hole is **very effective**: https://pi-hole.net/

These solutions offer huge savings in data and bandwidth, not to mention considerable energy savings.

For example, Pihole blocks 35-60% of advertising and trackers. This translates into a 50% increase in battery life for my Samsung smartphone.

I have created blocking lists for Pi-hole. You can download them to your computer and open them with your favourite editor.

* A list based on strict regexes of domain names [pihole_domains_list.txt](https://github.com/Vincent-Millane/cname-cloaking/blob/main/pihole_domains_list.txt)
* A list based on regexes that take sub-domains into account [pihole sub-domain list.txt](https://github.com/Vincent-Millane/cname-cloaking/blob/main/pihole%20sub-domain%20list.txt)

Do not add these lists as text lists because the regexes will probably be treated as text.

The solution, which only takes a few seconds, is to copy each list and paste it into the pihole graphical interface for adding regexes in :

_Domains > Domain management > RegEx filter_
and paste into the field.

Clicking on the _‘Add to denied domains’_ button will add the regexes to Gravity's sqlite3 database in a few seconds.   
You will notice that the red icon to the right of "Domains" has increased accordingly.

Pihole remains the ideal solution for protecting **all the devices in your home** as soon as you can specify a DNS server on your private network. 

Pihole even protects you outside your home if you use a VPN that connects you to your web router.

### Tips

- In my observations, I have found that it is risky to use Android applications that have hard-coded calls to trackers, bugs and advertising agencies. I assume the same applies to iPhones, but I don't have any to verify this.  
As far as possible, use a good browser with extensions that protect your privacy (high marks to ‘cookie autodelete’ for taking care of cookies). This will be enough to block all these malicious trackers, although there are a few caveats.

- It is possible that the regexes can block sub-domains of sites that you like with Pihole, the solution is to set the blocked line to ‘Allow’ to authorise this sub-domain.


## Extensions for Android and IOS devices

Starting with the excellent ublock origin <https://ublockorigin.com>.

I found a cool Privacy Badger extension <http://privacybadger.org> that doesn't block ads but all cnames and other vicious trackers.

To block advertising Adguard is stable.
In the advanced settings, there is a watchdog option to restart Adguard. 
This is very useful if you find that Android regularly disables Adguard. It's an admission that this software is powerful.

Adguard works on Android and IOS <https://adguard.com/fr/welcome.html>

If you're experiencing several thousand connection attempts a day to **mobile.pipe.aria.microsoft.com**, which are draining the resources of your installation as well as those of your smartphone, you can stop and then disable the _Link to Windows_ application on Android.  
On Android 15, go to Settings > Applications 
and search for the _Link to Windows_ application.  
This stops all connections immediately. 
If you need this app for any interaction with Windows, you can activate it for as long as you need, and deactivate it when you're done.  
This application contains trackers that do not justify the tsunami of connections. 


## Adguard for Android TV, Linux, Mac, Windows

Adguard blocks ads, trackers and phishing 
<https://adguard.com>

\
\
\
\
\
\
If you wish to value my work and my investment, you can do so in Monero crypto-currency with this account number:

> 8AwD8HWyj1KSePrnk3VmkLJf3QQYKCHKmHBCZw4YBqEsLQpApAYUjRzQFx8WEQQqz78QXptAJvHQMPB2vp94pxiZTwtput9

I appreciate it.


## License


 This listing in licensed creative commons. You can use it, modify it under the conditions of quoting me and the Creative Commons license.
 
 <p xmlns:dct="http://purl.org/dc/terms/" xmlns:vcard="http://www.w3.org/2001/vcard-rdf/3.0#">
  <a rel="license"
     href="http://creativecommons.org/publicdomain/zero/1.0/">
    <img src="http://i.creativecommons.org/p/zero/1.0/88x31.png" style="border-style: none;" alt="CC0" />
  </a>
  <br />
  To the extent possible under law,
  <a rel="dct:publisher"
     href="https://github.com/Vincent-Millane/cname-cloaking">
    <span property="dct:title">Vincent Millane</span></a>
  has waived all copyright and related or neighboring rights to
  <span property="dct:title">Sites using cname cloaking to block with unbound</span>.
This work is published from:
<span property="vcard:Country" datatype="dct:ISO3166"
      content="FR" about="https://github.com/Vincent-Millane/cname-cloaking">
  France</span>.

