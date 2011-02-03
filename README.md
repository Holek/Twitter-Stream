= Twitter Stream =
Contributors: veneficusunus, holek
Donate link: https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=N9Q2JG3DP4SNC
Tags: twitter
Requires at least: 2.8
Tested up to: 3.0.4
Stable tag: 2.1.8

It is an unofficial version of the [Twitter Stream](http://return-true.com/2009/12/wordpress-plugin-twitter-stream/) Wordpress plugin. I contribute my changes in here, because I coulnd't find the original public repository for the plugin.

Twitter Stream is a very simple Twitter plugin designed to show a users Twitter timeline. Also includes file caching to stop API overuse.

== Description ==

oAuth is now functioning correctly. After installing go to settings->twitter stream and follow the instructions to get started.

Twitter Stream is a simple plugin designed to simply show a users Twitter timeline. It includes file caching to stop overuse of Twitter's API. You can also choose how many updates to return (maximum of 200). It also includes autolinking for URL's found within the timeline. Also includes a date ago feature, showing the time the tweet was posted in xx ago format. Also has a permalink pointing to the tweet.

A widget is included, but you must have WordPress version 2.8 or higher for it to work, however function usage should work down to version 2.5 although it has not been tested.

Twitter Stream requires PHP5 due to the use of SimpleXML. If you do not have PHP5 installed you will not be able to use this plugin.

Twitter Stream is also designed to be very lightweight & use the smallest amount of resources possible, ideal for shared or low memory servers.

Here is a quick run down of the features available in Twitter Stream.

1. Show the twitter timeline for the oAuth athorized user or any public user.
2. Choose how many tweets to show.
3. A Widget or template function is available.
4. File caching to stop API overuse.
5. Optional date shown in xx ago format, also links to permalink for the tweet. (Requested by Ron)
6. Customizeable via CSS. (see 'Can I Style It?' in the FAQ)
7. Authentication for more accurate API counting & so protected users can show their tweets.
8. Translation files for different languages are now available to download on my [blog post](http://return-true.com/2009/12/ordpress-plugin-twitter-stream/ "Check here for translation files.").
9. @replies now link to the user profile of the user you are replying to.
10. #tags now link to the Twitter search page for that hash tag.
11. Link to user's profile, customizable via CSS & via function parameter.
12. Optional display of follower count.
13. Retweets can now be shown.
14. Cache time can be customized via the widget or template function.

A big thank you to all the people who have translated Twitter Stream into different languages.

1. [Fatcow](http://www.fatcow.com/)
2. [Tolingo.com](http://tolingo.com)
3. [Albert Johansson](http://twitter.com/albertjohansson)


== Installation ==

Download & install via the WordPress plugin repository in the admin of your blog, or you can do it the manual way as follows:

1. Go to your `wp-content/plugins` folder.
2.
    git clone git://github.com/Holek/Twitter-Stream.git twitter-stream
3. To use the Widget. Go to appearance, click widgets & drag it to a widgetized area of your choice & fill in the fields.
4. Go [here](http://return-true.com/2009/12/wordpress-plugin-twitter-stream/ "PHP function call") for info on how to use Twitter Stream in your template.

== Frequently Asked Questions ==

=== Can I Style It? ===
You can. I haven't added any styles so I could keep the plugin on one file & keep it free of clutter. The available CSS classes are:

1. .at-reply for @replys.
2. .hash-tag for #tags.
3. a.twitter-link for autolinked URL's within the timeline.
4. a:hover.twitter-link for autolinked URL's within the timeline when they are hovered over.
5. a.twitter-date</code> for the date permalink.
6. a:hover.twitter-date</code> for the date permalink when it's hovered over.
7. .profile-link for the newly added link to user profile.
8. .follower-count for the newly added follower count.


== Changelog ==

=== 2.1.8-git ===
* Holek: Adding hashtag recognition for Germanic umlauts

=== 2.1.8 ===
* Correct error cause by OAuth PECL being installed on server. I thought I'd fixed it but apparently not.

=== 2.1.7 ===
* Correct syntax error. Thanks Notepad++

=== 2.1.6 ===
* Check if OAuth is already available on server

=== 2.1.5 ===
* Now requires oAuth authorihttps://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=N9Q2JG3DP4SNCzation and added a custom cache timing.

=== 2.1.4 ===
* Added fix for those who's PHP install includes PECL oauth library

=== 2.1.3 ===
* Fixed extremely stupid mistake whiched stop oAuth from becoming active.

=== 2.1.2 ===
* Fixed problem that makes oAuth refuse connection with 401

=== 2.1.1 ===
* Correct an annoying SVN problem now have to create new version number to force update in WP admin for users of plugin.

=== 2.1 ===
* Reintroduced oAuth using user application registration method for consumer keys...

=== 2.0.2 ===
* Fixed cURL bug. curlopt_get is not needed as is set to get by default & it is curlopt_httpget...

=== 2.0.1 ===
* Removed oAuth until key exchange system does not make keys public...

=== 2.0 ===
* Version number change

=== 2.0-beta ===
* Changed authentication system to oAuth & made general improvements to the entire code.

=== 1.9.6 ===
* Once more, trying to fix ugly errors.

=== 1.9.5 ===
* Tried to fix ugly errors.

=== 1.9.4 ===
* Added TRUE to array_slice() to preserve the keys. How my localhost was preserving them without this option I'll never know. Thanks to Bryon Powell for the heads up.

=== 1.9.3 ===
* fixed an exceptionally stupid spelling mistake in a variable effecting the widgets. Thanks to fruityoaty for spotting the bug.

=== 1.9.2 ===
* Added back support for parameters, please use twitter_stream_args for array/query string support.

=== 1.9.1 ===
* Minor bug fix. Showed more tweets than specified count.

=== 1.9 ===
* Stopped function parameter support, now only support array or query based options. Also added follower count & retweet support.

=== 1.8 ===
* fixed some small errors.

=== 1.7 ===
* Fixed stupid widget HTML error that caused WP's text to go tiny.

=== 1.6 ===
* Added i18n pluralization support for xx ago time system.

=== 1.5 ===
* Added i18n support & Swedish .po file.

=== 1.4 ===
* Added a bug fix for some strange PHP bug. Bug number #36795...

=== 1.3 ===
* Added htmlentities() for escaping special characters such as ampersands etc..

=== 1.2 ===
* Added user authentication & more advanced error checking.

=== 1.1 ===
* Added date ago feature. Also added some minor fixes including PHP version checking & Username checking.

=== 1.0 ===
* Initial Release.
