=== Plugin Name ===
Contributors: mark8barnes, theKiwi, phaedrus428
Donate link: http://lisaandroger.com/downloads/
Tags: tng, the next generation, genealogy, integration, bridge, family history
Requires at least: 2.5
Tested up to: 4.7
Stable tag: trunk

Integrates TNG (The Next Generation) genealogy software into Wordpress.


== Description ==

[The Next Generation](http://lythgoes.net/genealogy/software.php) is a powerful PHP/MySQL script that acts as a central repository for all your genealogy research, and allows others to view and search through your records. This plugin integrates TNG with your Wordpress site. This plugin is free, but to use it you need to purchase TNG (currently $32.99).

#### Warning ####

Do NOT install this update if you are using TNG 9 or TNG 10.0

#### Note ####

The update of this plugin to Version 10.1.0 is to bring the version in line with compatible TNG Version numbers. The number 10.1.0 matches the minimum TNG Version that this plugin works with.

TNG-WordPress Plugin Version 10.1.x is compatible with TNG Version 10.1.x and TNG 11.x. It is NOT compatible with TNG 10.0.x or lower.

If you want to use this on TNG 10.0.x or 9.x.x then download and use [this version](https://downloads.wordpress.org/plugin/tng-wordpress-plugin.9.0.0.zip).

#### Features ####

1. Displays TNG within Wordpress with no iFrames (great for SEO!), on whichever page you choose.
2. Requires no mods, and overwrites no core files. Just upload the plugin to your Wordpress plugins folder.
3. Optionally puts the TNG menu into Wordpress sidebar, and optionally adds a search box there, too.
4. Optionally integrates Wordpress and TNG sign-on - effectively merges TNG and Wordpress users.
5. TNG and Wordpress are kept in separate folders for easy upgrading.
6. TNG and Wordpress can share the same database, or you can keep them separate.
7. Compatible with custom themes and TNG mods.

#### Demo ####

You can view this plugin in action at [Roger's Online Genealogy](http://lisaandroger.com/genealogy/getperson.php?personID=I16&tree=Roger)

#### Limitations ####

1. 'Pretty' permalinks must be turned on.
2. It may not work with IIS (Windows server).

== Installation ==

1. Upload TNG to your server if you’ve not already done so, and enter the database connection details in config.php. You’ll probably also need to change $rootpath to point to the folder you installed TNG in.
2. Create a blank page on your Wordpress site where you want TNG to be displayed. Unfortunately, this cannot be your home page.
3. Copy the tng-wordpress-plugin folder (from the plugin .zip file) into your Wordpress plugins folder (or use the install plugin option in Wordpress Admin).
4. Choose options from the new TNG menu that appears, and set the path to your TNG installation, and confirm the page you want TNG to be displayed on.
5. Add the TNG widgets at the top of your sidebar. By default they are displayed on your "not TNG" pages.
6. That’s it (hopefully!)
7. A comprehensive step by step is contained on the [TNG Wiki](http://tng.lythgoes.net/wiki/index.php?title=Using_TNG_and_WordPress_with_the_tng-wordpress-plugin)

== Screenshots ==

1. TNG 11.1 running inside the Suffusion WordPress theme. This shows an individual "getperson.php" page.
2. The WordPress Admin page for the TNG-WordPress Plugin showing the settings.

== Changelog ==

#### 10.1.1 ####
Changed Version number to force an update for those who already have 10.1.0. No code changes from 10.1.0 to 10.1.1

#### 10.1.0 ####
Version 10.1.0 is the current version for TNG 10.1.x and TNG 11. These changes are noted here to bring the Plugin Version numbering inline with TNG Version numbering.

Includes changes to replaced deprecated WordPress functions:
	ereg_replace is replaced by preg_replace;
	update_usermeta is replaced by update_user_meta;
	get_currentuserinfo is replaced by wp_get_current_user;
	delete_usermeta is replaced by delete_user_meta;
	The calls to mysql_xxx functions in the function mbtng_db_connect are replaced with tng_xxx calls for the new connection protocols introduced with TNG 10.1.0;
	Changes to use http/https as determined from the site's settings for compatibility with TNG's $http variable.

#### 9.0.0 ####
TNG-WordPress Plugin version 9.0.0 brings the version available on WordPress.org in line with the version that has been available for download from the TNG website.