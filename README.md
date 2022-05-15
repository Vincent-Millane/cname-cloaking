# Detailed list of sites using cname-cloacking with their extensions

__Sites using stalkers disguise with cname, a method to block them with Unbound__



## Why ?
Cname-cloacking is in violation of European laws (GDPR) and the law in many countries since they hide DNS referrals to the site you are visiting. It is therefore impossible to collect the user's consent for these third-party sites and the immediate effect is that you are tracked on all kinds of sites.

It is a more pernicious method than third-party cookies because it is unspoken and without recourse.
It's a real gold mine for companies that use this process.

These companies can keep your data as long as they want since this data does not officially exist. It could be our whole life.

Some cname lists that circulate on the internet are very superficial and masked by different acts.
In fact, an address can hide hundreds of addresses with extensions or referrals to other very interesting addresses.
 
Would you like to have a spy placed on your shoulder from morning to night to analyze your every movement of the day down to the brand of toilet paper you use?



## Method of working

List of cname-cloaking-blocklist quite detailed and classified by domain name with its extensions.

I am in the process of completing it and there is a lot of work.

It is useful to realize that behind a .com domain name companies can hide hundreds or thousands of subdomains, for example __custom.com hides 33,243 subdomain names__. Blocking by domain name extensions makes perfect sense.



## Install Recursive Cache DNS Server

### Where download Unbound ?

This list is in the stub-zone format of Windows, Linux and BSD compatible unbound software (https://nlnetlabs.nl/projects/unbound/about/).

Under linux, Unbound is probably available in packages. Search with apt, yum or dnf.

### Unbound configuration
 
To configure Unbound according to your needs with several examples configurations: https://calomel.org/unbound_dns.html.

#### Configure unbound.conf with this stub-zone list
 
To save this list in the /etc/unbound folder

    sudo gedit /home/path/to/your brand new stub-zone_file

and save to /etc/unbound/ directory

open your configuration file

    sudo gedit /etc/unbound/unbound.conf 

and add towards the end of your file:

> include: "/etc/unbound/stub-zone" 

and save your file.

I recommend that you do a:

    sudo unbound-checkconf /etc/unbound/unbound.conf

to verify that there is no typo. 

#### Restart Unbound to take changes into account

then restart unbound with

    sudo systemctl restart unbound

to check that everything is going well

    sudo systemctl status unbound

and your anti-tracker list is operational immediately. It's normal if your web surfing is faster.

You will notice on the chrome browser, it displays more and more white area with dns errors.
Don't worry, it's a sign that these blocking rules are working properly, but also that companies have moved to trackink images that hide links.



## About this data

The data in this list is public and accessible to anyone who can use a DNS query tool such as nslookup, dig or drill, etc. and their graphic counterparts.

 Some web pages will go from 10 mb to 1 mb! (https://www.laquadrature.net/2020/10/05/le-deguisement-des-trackers-par-cname/)

I was inspired in part by the work of these contributors https://github.com/nextdns/cname-cloaking-blocklist.
I use lists available on the web.
I dug deeper.

Feel free to share with me if you know of other sites, I will update my stub-zone.



## For Android devices

There is the application: __Blokada__ (https://blokada.org/) downloadable from the F-Droid repository (https://f-droid.org/). It is a trusted repository of free software and often of very good quality.


I have been using __Blokada__ since the beginning of January 2022, it has blocked 252,452 ads or trackers for me since. It has an option to activate to block cname trackers. That's an average of 2,019 blocks per day. Very convenient.



## Maybe I need help

Note: if someone is willing to translate this document for me into correct English, I would be delighted.
There you have English "made in Google".



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

