=== Dragon Video ===
Contributors: DexterTheDragon
Tags: html5, video
Requires at least: 3.5
Tested up to: 3.9
Stable tag: 1.0.1
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

A WordPress plugin for converting uploaded videos to HTML5 format (h264, webm, ogv) and displaying them with the <video> tag.

== Description ==

A WordPress plugin for converting uploaded videos to HTML5 format (h264,
webm, ogv) and displaying them with the <video> tag.

Dragon Video consists of 3 plugins:

* Dragon Video
* Dragon Video - Zencoder encoder
* Dragon Video - VideoJS Player

Dragon Video is the core plugin. It handles interfacing with videos
uploaded through WordPress, passing them off to an encoder, providing a
shortcode to display the video, and enabling videos to be shown in the
WordPress gallery. Dragon Video itself does not handle video encoding.
WordPress actions are called for video encoding and display of the HTML5
tag allowing any desired encoder or player to be used.

Dragon Video - Zencoder encoder is a bundled encoder. It uses
http://zencoder.com to encode uploaded videos to HTML5 media types. An
API key is required to use.

Dragon Video - VideoJS Player is a bundled player using the
http://videojs.com/ HTML5 video player.

== Installation ==

1. Unzip the package and upload the dragon-video directory into your wp-content/plugins directory
1. Activate the plugin at the plugin administration page

== Screenshots ==

1. Dragon Video Options Page
2. Zencoder Options Page

== Changelog ==

= 1.0.1 / 2013-07-09 =

 * Include videojs files

= 1.0.0 / 2013-07-08 =

 * Add WordPress plugin readme
 * Hopefully fix travis config
 * More badges
 * Set coveralls json_path
 * Merge branch 'refactor'
 * Allow build failures on WordPress master
 * Reorganize tests
 * Add namespace
 * PSR Styling
 * Remove assign by reference
 * Split is dericated, use explode instead
 * Clean up some code
 * Fix plugin activiation after refactor changes
 * Drop WP 3.4/3.3 support
 * Upgrade video.js to 4.0
 * Fix paths in test
 * Test coverage for ZencoderEncoder::_handle_incoming_video
 * Update composer.lock
 * Upgrade to v2 of Zencoder API
 * Add coveralls.io config
 * Move tests to test
 * Cleanup tests
 * Reorganize files
 * Add tests for ZencoderEncoder
 * Add tests for VideoJsPlayer
 * Fix test for multisite
 * Install ffmpeg on travis
 * Add build status image
 * Add travis-ci config file
 * Add tests for DragonVideo

= 0.9.0 / 2013-04-25 =

* Update for WordPress 3.5 galleries

= 0.5.0 / 2012-01-16 =

* Allow shortcode to specify size
* Fix delete attachment bugs
* Move encoder/player plugins out of subfolders
* Pass post id instead of object
* Move add_option to activate
* Change all instances of ogg to ogv, fix unset var notices
* Refactor zencoder code, add option page
* Cleanup code, add options page

= 0.4.0 / 2010-12-25 =

* Upgrade video.js
* Fix video gallery
* Add default loader plugins
* All videojs stuff
* only run delete if its a video
* Setup player to display mp4, webm, and ogg
* Use medium as size
* Add class to video attachment link
* Streamline size storage and retrieval
