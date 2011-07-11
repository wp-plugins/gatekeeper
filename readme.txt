=== Plugin Name ===
Contributors: jamiewilson
Donate link: https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J3ETMQWMPY586
Tags: gatekeeper, offline, maintenance, whitelist, blacklist, access, ip, coming soon
Requires at least: 3.0
Tested up to: 3.3
Stable tag: 0.8

Gatekeeper allows administrators to take a WordPress site offline while leaving it accessible to authorized users for maintenance, testing, etc.

== Description ==

Gatekeeper allows administrators to take a WordPress site offline quickly and easily while leaving it fully accessible to administrators and other authorized users. Site visitors will be shown or redirected to a specified offline page. An optional blacklist can be used for permanent bans.

** Features **

* Visitors can either be redirected to an existing non-WordPress offline page (using http 302 temporary redirect) or WordPress pages can be temporarily replaced with the offline page.
* Logged in admins can be whitelisted
* The current admin's IP address can be automatically whitelisted
* An IP-based whitelist that can accept specific IP addresses, wildcards, and ranges
* An IP-based blacklist that redirects blacklisted IPs to a specified page
* A notifier that appears on administrator pages when the site is offline

== Installation ==

1. Upload `gatekeeper` to the `/wp-content/plugins/` directory.
1. Activate the plugin through the 'Plugins' menu in WordPress.
1. Go to <em>Tools > Gatekeeper</em> to manage Gatekeeper.


== Frequently Asked Questions ==

= Why was this plugin developed? =

I needed a "coming soon" page for a site I was working on but also needed to be able to use WordPress myself in order to test themes, designs, etc.
The existing landing page themes are nice, unless you also need to be able to test a theme without letting the world see. At first, I added some PHP 
code into the WordPress index.php file to redirect all but my IP address to the coming soon page, but WP upgrades opened my site to the world. Editing 
the htaccess file is an option, but it's extra work and only works until my IP address changes. So...I created Gatekeeper.

= Can I redirect visitors to an existing WordPress page? =

No. Gatekeeper protects all WordPress pages (except admin and login pages) from everyone but those whitelisted, so redirecting to a WordPress page
would create an undesirable redirect loop.

= Can Gatekeeper protect non-WordPress pages? =

No. 

== Screenshots ==

1. The Gatekeeper administration page

== Changelog ==

= 0.8 =
* First release candidate.

== Upgrade Notice ==

* No upgrades available.