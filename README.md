# cname-cloaking
Sites using cloaking cname to block with unbound

Cname-cloacking is in violation of European laws (GDPR) and the law in many countries since they hide DNS referrals to the site you are visiting. It is therefore impossible to collect the user's consent for these third-party sites and the immediate effect is that you are tracked on all kinds of sites.

It is a more pernicious method than third-party cookies because it is unspoken and without recourse.
  
 It's a real gold mine for companies that use this process.
 
 Would you like to have a spy placed on your shoulder from morning to night to analyze your every movement of the day down to the brand of toilet paper you use?

 List of cname-cloaking-blocklist quite detailed and classified by domain name with its extensions.

I am in the process of completing it and there is a lot of work.

 This list is in the stub-zone format of Windows, Linux and BSD compatible unbound software (https://nlnetlabs.nl/projects/unbound/about/).
 
 To configure Unbound according to your needs with several examples configurations: https://calomel.org/unbound_dns.html
 
 To save this list in the /etc/unbound folder
sudo gedit /home/path/to/your brand new stub-zone file and save to /etc/unbound/
open and add towards the end of your file:
include: "/etc/unbound/stub-zone" and save your doc

 I recommend that you do a:

sudo unbound-checkconf /etc/unbound/unbound.conf

 to verify that there is no typo, then restart unbound with

 sudo systemctl restart unbound

 to check that everything is going well

 sudo systemctl status unbound

 and your anti-tracker list is operational immediately.

 The data in this list is public and accessible to anyone who can use a DNS query tool such as nslookup, dig or drill, etc. and their graphic counterparts.

 Some web pages will go from 10 mb to 1 mb! (https://www.laquadrature.net/2020/10/05/le-deguisement-des-trackers-par-cname/)

I was inspired in part by the work of these contributors https://github.com/nextdns/cname-cloaking-blocklist.
I use lists available on the web.
I dug deeper.
 
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

