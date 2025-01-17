=== WP Inline Access ===
Contributors: mrwweb
Tags: Inline Access, Editing, Admin, Front End Access
Requires at least: Unknown
Tested up to: 3.6
Stable tag: 0.6.0
License: GPLv2 or later

An alternative to front end editing. Click on an element, teleport to the right admin screen.

== Description ==

**NEW ARTICLE** [Lessons learned so far and user survey.](http://mrwweb.com/wp-inline-access-future/) Please take it!

([Original Proposal Article](http://mrwweb.com/wp-inline-access/))

**THIS PLUGIN IS AN ALPHA RELEASE. USE AT OWN RISK AND TELL ME HOW TO MAKE IT BETTER (or [contribute on GitHub](https://github.com/mrwweb/wp-inline-access)).**

Front end (or "inline") editing sounds great until you try to apply it to large complex CMS sites. Rather than try to keep users out of the admin because they can't understand it, why not build an editing system that teaches them how to use it?

This plugin is designed to work best in conjunction with [MP6](http://wordpress.org/plugins/mp6/) or WP3.8+ and one of the tested themes below.

= Editable Items Supported =
* Menus (`wp_nav_menu`)
* Widgets (`dynamic_sidebar`)
* Site Description ("Tagline", `get_bloginfo`)
* Body Content (`the_content`)
* Featured Image (aka Post Thumbnail, `the_post_thubnail`)
* Excerpt (`the_excerpt`)
* Tags (`the_tags`)
* Categories (`the_category`)

= Info Bar Information =
* Page Type (aka Post Type, Archive, Page for Posts, 404, Search Results, etc.)
* Page Template (when appropriate)
* Page Parent
* Post Format
* Post Type Archive Post Type
* Page on Front and Page for Posts settings
* Last Modified / Published Datetime
* Taxonomy Term Archive Term (Tag, Category, custom, Post Format)
* Posts Per Page

= Tested Browsers =
* Chrome

= Themes Tested =
* Twenty Twelve
* Twenty Eleven
* Twenty Ten

== Installation ==

= Manual =
1. Download plugin zip file.
1. Unzip into your site's `/wp-content/plugins/` folder.
1. Go to Plugins in Dashboard.
1. Activate "WP Inline Access."

= Automatic =
1. In the Dashboard, go to Plugins > Add News.
1. Search for "WP Inline Access."
1. Install plugin.
1. Activate plugin.

= Usage =
Once installed, click the "Toggle Edit Mode" button in the Admin Bar to display the Info Bar and editable page elements.

== Frequently Asked Questions ==

= So I can click on something and change the text right there? =
No. All editing is still done in the admin. This is NOT front end editing.

= What's your goal for this plugin =

This plugin is a proof of concept for something that, if I dream big, might make it into WordPress Core someday. Until then, you probably shouldn't use this on a production site without understanding the risks of using a plugin in early development stages.

== Screenshots ==

1. This plugin creates a new "Toggle Edit Mode" button in the Admin Bar. Click it to learn about the web page you're viewing and enable clickable, editable elements.
2. Once clicked on the front end, the clicked element is highlighted. (Widgets are especially pretty.)

== Changelog ==

= 0.6.0 (November 14, 2013) =
* New ["Lessons Learned and User Survey"](http://mrwweb.com/wp-inline-access-future/) post. Please read and fill out!
* Posts Per Page now show in Info Bar when appropriate
* Permissions check for infobar, editable values
* Hide Info Bar on small screens for now (following MP6's lead here)
* Improve multi-line Info Bar display

= 0.5.0 (November 8, 2013) =
* Capability checks on all editable elements.
* Don't create empty editable items. (Refactored basic helper functions.)
* [Temporarily?] Prevent nested editable elements.
* Support for inline, inline-block, and block editable elements. Previously everything was forced to `display:block;`
* More info in the Info Bar: Page Parent, Published/Updated Datetime, Term for Term/Tag/Category/Post Format archives
* MP6 Style Fixes: widget admin updates
* No-MP6 Style Fixes: Admin bar height and widget highlighting

= 0.4.0 (October 27, 2013) =
* More info in the Info Bar: Post Format (archive and single post), Page for Posts option
* Regression: Widget highlighting doesn't work with new versions of MP6 / Features as Plugin Widget admin plugins.

= 0.3.0 (October 18, 2013) =
* Newly editable fields: Excerpt, Featured Image, Categories, Tags
* New styles for targeted metaboxes on the admin
* Dims images in editable elements when hovered
* Don't allow editable elements in the admin

= 0.2.0 (October 10, 2013) =
* Zoom to and highlight clicked edit in admin.
* "Site description" is now editable
* Improved CSS: Highlight targeted text inputs.
* More bulletproof front-end CSS. Including Twenty Eleven fix.
* anything outputted with `the_content` is now editable.
* Hi, #wpseattle!

= 0.1.0 (October 7, 2013) =
* Alpha Release

== Upgrade Notice ==
= 0.6.0 =
Info Bar improvements. Check out the update article & survey in the changelog!

= 0.5.0 =
TONS of improvements! New info. Safer editing. Cleaner editable styles. Widget style fixes.

= 0.4.0 =
More info in the Info Bar.

= 0.2.0 =
Highlight clicked element in dashboard. Content and Tagline are editable. CSS improvements. See changelog for deets.

= 0.1.0 =
You can't upgrade to this because nothing precedes it. Deep.