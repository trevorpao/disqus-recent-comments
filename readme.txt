=== Recent Comments from Disqus ===
Contributors: MediaMisfit
Donate link: 
Tags: comments
Requires at least: 3.3
Tested up to: 3.5.1
Stable tag: 
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

A WordPress(WP) sidebar widget that displays the most recent comments made using Disqus (http://disqus.com). 

== Description ==

A WordPress(WP) sidebar widget that displays the most recent comments made using Disqus (http://disqus.com). Settings include an optional title and results threshold from 5-10.



== What is required? ==

* [Disqus Comment System](http://wordpress.org/extend/plugins/disqus-comment-system/ "Disqus Comment System").
* Public API key from a [Disqus API application](http://disqus.com/api/applications/ "Disqus API application").


== Installation Steps ==

* Copy the plugin to your /wp-content/plugins directory. 
* Activate the plugin with your WordPress control panel. 
* Initiate the widget by adding it to your layout via the WP widget menu.


== How does it work? ==

On activation a new database(db) table with 10 rows is created to house your comment results. The widget checks for the required Disqus plugin and API key. If they're unavailable you'll be prompted and the widget won't display.

After the widget has been initiated (by being added to your layout), an API call will be made to grab and store the following information for the 10 latest comments:

* Thread Title
* Message
* Comment URL
* Thread URL
* Author Name
* Comment Date

A 60 second WP_cron will keep your list current.


== Details ==

Date format: Month day, Year

Substring thresholds: 

* Title - 30 chars
* Comment - 120 chars


== Customization ==

style.css provided