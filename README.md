# S4 - Open Source Philosophy

A list of the open source services and systems we use to run S4 Sustainable Hosting.

At S4 we believe in accountability, transparancy and open source software. We also believe in a lot of other things, but those are the most relevant to this document. We have chosen to make this list publicly visible so you can see how we are running and constantly developing our hosting platform. Some people might argue that this is a bad idea for 'security through obscurity' reasons, but we disagree.  

Our main services are all hosted at the sustainalbe Telia Helsinki Data Centre, with backups and utilities hosted at a sustainable Ineterxion data centre in Amsterdam.

* Our web servers are CentOS and run Open Litespeed or LiteSpeed Enterprise web server, with Cyberpanel as a control panel. 
* Our mail servers are Ubuntu and are running our customised version of Mail-in-a-box. 
* Our analytics servers are CentOS, running OpenLiteSpeed and Matomo analytics.
* Our utilities server running various monitoring services is Ubuntu and runs Statping as an uptime monitor.

---

### Projects we actively use...

#### Matomo - https://github.com/matomo-org/matomo
For all of the obvious data privacy and ownership reasons we don't use Google Analytics or similar, but instead install ethical analytics on our own sustainably hosted servers. There are a few options, Matomo is the best we've found so far. 

*We maintain our own Matomo Tracking plugin for S4 Hosting clients.*

#### Statping - https://github.com/statping/statping
We want to love Statping so much, it's the uptime monitor and status page generator that we are using at the moment, but it's not quite where we would like it to be

#### Mail in a Box - https://github.com/mail-in-a-box/mailinabox
Running and maintaining a mail server with high deliverabilty is hard and time consuming, but at least you can make sure that setting one up is quick, easy and done right. We love MIAB and it's what we use as a base for all of mail servers. 

#### Open LiteSpeed - https://github.com/litespeedtech/openlitespeed
LiteSpeed is great, both OLS and Enterprise LSWS. They are what all of our web servers run on. It's not a decision that we took lightly, having run tests on Apache and Nginx as well, but one that had a clear winner for us.

#### CyberPanel - https://github.com/usmannasir/cyberpanel
Is CyberPanel perfect, is each update entirely free of bugs, is it more fully featured than all of the other control panels out there, is the UI beautiful? No, to all of those. It is developing very quickly with devs who do actually listen, becoming more stable and feature-rich all the time, and is the native control panel for LiteSpeed, which makes it an obvious choice for us. 

#### MainWP - https://github.com/mainwp/mainwp
We administer a lot of WordPress sites and we've built our own process and system for keeping tabs on updates, security issues, backups, etc. across our own and clients sites. At the core of this we use MainWP, which is the best solution we've found for remotely administering multiple WP installations. 

*We maintain our own fork of the MainWP Child plugin for S4 Hosting clients.*

#### Flarum - https://github.com/flarum
Flarum is modern forum software, similar in many ways to Discourse but written in PHP and much less recource hungry, it's lightweight, fast and extensible. It is currently our go-to forum solution for client sites. 

---

### ...and ones we are watching

#### Open Web Analytics - https://github.com/Open-Web-Analytics/Open-Web-Analytics
We really like the look of OWA but haven't found the time to thoroughly test it out yet. 

#### Plausible Analytics - https://github.com/plausible/analytics/
Another really interesting ethical analytics solution that we need to find the time to test out thoroughly. 

#### Cachet - https://github.com/CachetHQ/Cachet
Cachet is the other alternative that we looked at when we chose to run Statping. Neither is perfect for us and it could have gone either way. We will keep an eye on Cachet and won't rule out swtitching in the future. 

#### Boxbilling - https://github.com/boxbilling/boxbilling
We don't actually use any of the usual billing/automation solutions, i.e. WHMS, Blesta. Instead we use our own solution that works for us but quite honestly could be better and that we are spending a lot of time improving. If there was a reliable, secure open source altherantive that we could use to build on then that would be wonderful, but right now there isn't. What there is, is boxbilling, a project that seemed viable and showed a lot of promise about 6 years ago but then seemed to hvae died. It's finally been updated to PHP 7 from 5.6 recently and maybe there is hope that something can rise from it. We wouldn't consider using it for production right now, but we are glad it's still kinda alive. 
