=== Enhanced Media Library ===
Contributors: webbistro
Tags: media library, media category, media categories, media management, media organizer, media gallery, gallery shortcode, media tag, media tags, media taxonomy, media taxonomies, media uploader, mime type, mime, mime types, file types, media types, media filter, attachment, gallery, image, images, media, ux, user experience, wp-admin, admin, taxonomy, taxonomies
Requires at least: 4.0
Tested up to: 4.4
Stable tag: 2.1.3
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html



A better management for WordPress Media Library



== Description ==

The plugin will be handy for those who need to manage a lot of media files.


= Media Taxonomies (Categories and Tags for media files) =

With the plugin installed you will immediately obtain Media Categories that will be useful for categorizing and filtering media items in the WordPress admin. This feature alone will save you hours of searching through a media library with even as few as 100 images.

Whether you have a lot of images that need to be organized into complex structures or simply dislike the name of the default taxonomy - Media Categories - you can create and (un)assign to the media library as many taxonomies as you wish without writing a single line of code. Even in case the only taxonomy is totally enough for you, you may prefer to call it "Photo Categories" or simply "Photos".

You can also assign to the media library built-in WordPress taxonomies - Categories and Tags - as well as any other taxonomy created by third-party plugin, theme, or hand-coded with only plugin's UI.

The plugin will allow you to categorize both new and existing media items. You can assign a category to a media item during the upload process, in the media library (preferably Grid Mode), in the post/page editor media popup ("Add Media" button). If you need to manage a lot of media items at once, there is the PRO version of the plugin that allows to do it in bulk.

Every media library window is enhanced with the plugin's filters to search and sort your media files. With the flexible plugin's options you can adjust what filters you will see in the Grid and List modes of the media library and in the post/page editor media popups, and what taxonomies you would like to be able to edit when inserting media to posts/pages. The plugin will work with custom post types as well. The options will also help you to force plugin's filters for third-party plugins or themes, manage media taxonomies archive pages, etc.

Since the version 2.1 you can change the order of media items within a category with drag and drop. This order will be used, in particular, for the gallery based on this category.


= Filter-Based Image Galleries (Fully compatible with WordPress native gallery shortcode) =

Image categorizing can be useful for the front-end, of course. To insert media galleries based on media categories you have to use the familiar format like `[gallery media_category="5" category="2" monthnum="12" year="2015" orderby="title" order="DESC"]`. The PRO version of the plugin allows to manage gallery shortcode without "coding" at all. Just choose the settings with the plugin's UI in the familiar gallery edit popup and see your gallery live immediately in the post/page editor.


= MIME Types (Media File Types) =

Another feature of the plugin is the MIME Types control. You can add new MIME types, delete existing ones, and point what file types are allowed for uploading. Initially, the plugin shows up the WordPress default MIME Type settings and creates the backup of them. The column "Add Filter" allows to add a MIME Type to plugin's filters so that you will be able to filter your media items not only by categories but also by the file type. You can set any label you wish to see in a filter with columns "Singular Label" and "Plural Label".


= Export / Import Plugin Settings =

If you need to move your media library to another website you should export and import WordPress content with WordPress built-in export/import. But to make the Enhanced Media Library work on the new site with the same settings you are provided with the export/import feature.


= Easy to Use and WordPress Native Functionality Oriented Plugin =

We spend hours to make plugins features work as though they were native WordPress functionality. If you are a developer and looking for a solution totally compatible with WordPress core and, at the same point, really easy to deal with for your non-geeky customers, give it a try, you won't be disappointed.


= Support =

Support is free for both versions of the plugin. "PRO"-users do not have priority. We do out best to respond in 24 hours if not sooner.


= Available Languages (Assistance with the translation is highly appreciated) =

* Dutch
* German
* Hebrew
* Korean
* Polish
* Swedish

Many thanks to the authors of the translations! If you wish to be credited here please just let us know what name and URL we have to use.


= Compatibility with Other Plugins =

* Advanced Custom Fields
* Search & Filter
* Jetpack Carousel
* WooCommerce
* Meta Slider

Please let us know if you find any issue with the plugins from the list above or others.


= Incompatibility =

Please notice that you use the Enhanced Media Library with other plugins that add media categories, media folders, and manage MIME Types at your own risk. We cannot guarantee their compatibility because of different approach to the same functionality. It does NOT mean that we do not recommend using those plugins, it just means we do not recommend to use them at the same time with the Enhanced Media Library. Please choose the one you prefer.


> #### Enhanced Media Library PRO

> The key features:

> * Media files can be categorized in bulk (multiple files to multiple taxonomies at once) both just uploaded and existing
> * Media files within a category can be selected in bulk with a single click
> * Selected media files can be deleted in bulk in the Grid mode of the media library or in the post/page editor media popup
> * Filter-based gallery in two clicks, no need to figure out your media category IDs, nor to delve into the text editor shortcode


= Useful Links =

* [Where to start? (The complete beginners guide)](http://wpuxsolutions.com/documents/enhanced-media-library/eml-where-to-start/)



== Installation ==

1. Upload plugin folder to '/wp-content/plugins/' directory

2. Activate the plugin through 'Plugins' menu in WordPress admin

3. Adjust plugin's settings on **Media Settings >> Taxonomies** or **Media Settings >> MIME Types**

4. Enjoy Enhanced Media Library!



== Frequently Asked Questions ==

= Why my custom media taxonomy's page is 404? =

Try to just re-save permalinks settings. Go to Settings >> Permalinks and push "Save Changes" button.

= Why Media Popup of some theme/plugin does not show taxonomy filters? =

[**UPD:** Since EML 2.0.4 there is an option 'Force filters' (see Media Settings > Taxonomies) that allows forcing media filters for ANY Media Popup regardless of what was intended by the author of a third-party plugin or theme.]

EML adds its filters to ANY media popup that already contains native WordPress filters. We chose NOT to force adding filters to ANY media popup because there are a lot of cases when filters are not acceptable and theme's/plugin's author did not add them intentionally.

If you believe that a third-party plugin should have filters in its Media Popup please contact its author with a request to add NATIVE WordPress filters ([example of the code](http://wordpress.org/support/topic/how-can-we-use-this-plugin-features-in-my-custom-plugin-media-uploader?replies=15#post-5753212) for theme's/plugin's authors).

= How to show images per media category on a webpage? =

[**UPD:** Since EML 2.1 you can use gallery shortcode with taxonomy parameters like this: `[gallery media_category="5" category="2" monthnum="12" year="2015" orderby="title" order="DESC"]` to show filter-based gallery on the front-end.]

Right now it is possible via WP_Query ([example of the code](http://wordpress.org/support/topic/php-displaying-an-array-of-images-per-category-or-categories)). We are working on a gallery based on EML taxonomies.

= My gallery behavior is strange | My ligthbox/carousel plugin no longer works =

The Enhanced Media Library enhances the WordPress gallery shortcode with the 'post_gallery' filter. It does this in the most gentle manner possible. It overrides the database query and leaves HTML/CSS code generating intact.

But many other plugins do the same. Since, currently in WordPress it is not possible to separate a pure database request and generating gallery's HTML/CSS, the plugin conflicts are inevitable.

The solution: please visit Media Settings > Taxonomies > Optons and set "Turn off enhanced gallery". This will deactivate the gallery feature only without deactivating all other plugin's functionality. Then please let us know what functionality was broken. We would like to find a solution!

= Will I lose media categories I’ve created if I upgrade from free to PRO? =

No, all your data will remain intact. Your created media categories and their ties with your images are stored in the database. When you deactivate and delete the free version and then upload and activate the PRO one nothing happens to the database.



== Screenshots ==

1. Media Taxonomies Settings

2. MIME types manager

3. Create media categories just like any others

4. Use media categories in Nav Menu

5. Attach media categories to media files like to posts

6. Attach media categories to media files from Media Library grid view

7. Attach media categories to media files in Media Popup while editing posts and pages. Filter media files by categories and file types

8. Filter media files by categories and file types in Media Library list view

9. Filter media files by categories and file types in Media Library grid view



== Changelog ==

= 2.1.3 =
*Release Date - December 17, 2015*

= Bugfixes =
* Compatibility of the plugin's code with different PHP versions ensured
* "Warning: Missing argument 3 for wpuxss_eml_gallery_shortcode()" fixed
* The bug with unavailable image meta on Edit Gallery screen fixed

= Improvements =
* "Turn off enhanced gallery" option added. Allows to turn off the gallery shortcode enhancement without deactivating the whole plugin in case of incompatibility with other plugins or themes. Please inform plugin authors about the issue. We would like to fix it!


&nbsp;
= 2.1.2 =
*Release Date - December 15, 2015*

= Compatibility =
* Fixed v2.1 and Jetpack Carousel incompatibility


&nbsp;
= 2.1.1 =
*Release Date - December 15, 2015*

= Bugfixes =
* Minor incompatibility with WordPress 4.3 fixed


&nbsp;
= 2.1 =
*Release Date - December 15, 2015*

= New =
* Filter-based Image Galleries by extending native WordPress gallery shortcode
* Easy visual gallery editing with the native WordPress gallery UI [PRO only]
* Export/import of the plugin settings to JSON

= Improvements =
* Better filtering and "force filters" mechanism, sorting by 'menuOrder' by default for media taxonomy filters
* Plugin credits in admin removed from Media Settings > Taxonomies, and Media Settings > MIME Types, moved to Settings > Enhanced Media Library
* "Deactivate License" added [PRO only]
* Various code improvements for both free and PRO
* Minor UX improvements

= Compatibility =
* Fixed incompatibility with [WP Plugin Dependencies](https://github.com/xwp/wp-plugin-dependencies)
* Wordpress 4.4 compatibility ensured

= Languages =
* Korean translation added


&nbsp;
= 2.0.4.8 =
*Release Date - September 14, 2015*

= Bugfixes =
* The bug with empty taxonomy drop down fixed
* WordPress 4.3 gallery's template issue fixed [Support Request](https://wordpress.org/support/topic/unable-to-remove-images-from-gallery)
* The bug with plugin's folder name fixed (PRO only)
* Minor WP 4.3 CSS compatibility issues fixed


&nbsp;
= 2.0.4.7 =
*Release Date - August 11, 2015*

= Bugfixes =
* Detach issue fixed [Support Request](https://wordpress.org/support/topic/cannot-detach-image-from-custom-post-type)
* The bug of load-upload.php hook fixed, please use any priority less than 999 for this hook
* Visual Composer incompatibility fixed (PRO only)

= Improvements =
* Better CSS for the Media Library grid mode (PRO only)
* Better localization [Support Request](https://wordpress.org/support/topic/the-plugin-codestyling-localization-was-forced-to-protect-its-own-page)

= Compatibility =
* Wordpress 4.3 compatibility ensured
* Visual Composer incompatibility fixed (PRO only)

= Languages =
* Hebrew translation added
* German translation added
* Swedish translation added


&nbsp;
= 2.0.4.6 =
*Release Date - April 29, 2015*

= Bugfixes =
* wp_dropdown_categories bug fixed [Support Request](https://wordpress.org/support/topic/wp_dropdown_categories-broken-with-2045)
* Few minor bug fixes


&nbsp;
= 2.0.4.5 =
*Release Date - April 24, 2015*

= Compatibility =
* Wordpress 4.2 compatibility ensured

= Bugfixes =
* Blank (empty) media library screen fixed for List and Grid views


&nbsp;
= 2.0.4.3 =
*Release Date - March 21, 2015*

= Bugfixes =
* List View: Incorrect filtration for post tags fixed
* Media > Add New: Incorrect media files selection (multiple uploading) fixed (PRO only)
* Edit details for all media file types fixed (PRO only) [Support Request](https://wordpress.org/support/topic/edit-video-detail-missing)
* Other minor bug fixes


&nbsp;
= 2.0.4.2 =
*Release Date - March 09, 2015*

= Bugfixes =
* The bug with "Fatal error: Call to undefined function get_userdata() in /wp-includes/user.php on line 360" fixed [Support Request](https://wordpress.org/support/topic/error-message-after-updating-3)
* The bug with incorrect filtering in Media Library List View fixed (when clicking directly on a media category name)


&nbsp;
= 2.0.4.1 =
*Release Date - March 07, 2015*

= Bugfixes =
* Plugin's options incorrect setting during update fixed. If your front-end media taxonomy archive pages were broken by the recent two updates, please re-save your Settings > Permalinks options
* The bug with "Fatal error: Call to undefined function ..." for Media Library List View fixed


&nbsp;
= 2.0.4 =
*Release Date - March 05, 2015*

= New =
* Filters by 'All Uncategorized', 'All Media Categories', 'Not in Media Category' added to both List and Grid views and to Media Popup
* New Media Taxonomy option: 'Edit in Media Popup' - Allows to show/hide taxonomy checkboxes in Media Popup per taxonomy.
* New Media Taxonomy option: 'Taxonomy archive pages' - Turn on/off taxonomy archive pages on the front-end
* New Media Taxonomy option: 'Assign all like hierarchical' - Allows editing of non-hierarchical taxonomies like hierarchical (checkbox list) in Grid View / Media Popup
* New Media Taxonomy option: 'Force filters' - Shows media filters for ANY Media Popup. May be useful for those who need to force filters for third-party plugins or themes

= Improvements =
* Admin Menu: All Media Settings including native 'Settings > Media' are now under common 'Media Settings' admin menu
* Bulk Edit options are now on 'Media Settings > Taxonomies' admin page
* CSS: Media taxonomies column extended for Media Popup, and few more minor CSS improvements
* Taxonomy Saving: Saving changes on the fly displays changes more correctly now (PRO only)
* Taxonomy Saving: Improved media taxonomies saving mechanism (better compatibility with other plugins, etc.)
* Numerous minor code and performance improvements

= Bugfixes =
* Taxonomy Saving: Fixed a big issue with incorrect bulk saving for media taxonomies (wrong clean-up for non-heirarchical taxonomies, PRO only)
* Taxonomy slug: Bug with the incorrect saving of a taxonomy slug fixed [Support Request](https://wordpress.org/support/topic/not-work-slug)
* Meta Slider plugin compatibility ensured [Support Request](https://wordpress.org/support/topic/filter-not-appearing-when-adding-slides-to-meta-slider)
* Localization: small localization bug fixed (PRO only)
* CSS: Admin notices layout fixed for the Grid View (PRO only)
* CSS: Incorrect checkbox styling for mobile devices fixed
* CSS: Few more minor CSS fixes


&nbsp;
= 2.0.3 =
*Release Date - December 19, 2014*

= Improvements (PRO only) =
* Bulk Edit added to the List View of Media Library
* Bulk Edit Media Popup (for Media Library > List View and Media Library > Add New page) is now being opened with pre-selected multiple media files

= Compatibility =
* Wordpress 4.1 compatibility ensured
* Improved compatibility with other plugins and custom taxonomies

= Bugfixes =
* "PHP Fatal Error: Call to undefined function get_current_screen()" issue fixed
* Minor bugs fixed


&nbsp;
= 2.0.2.3 (PRO only) =
*Release Date - November 27, 2014*

= Bugfixes =
* ACF: Fixed the bug with ACF < 5.0 compatibility


&nbsp;
= 2.0.2.2 =
*Release Date - November 23, 2014*

= Bugfixes =
* Minor JS bug of v2.0 fixed [Support Request](https://wordpress.org/support/topic/upload-hangs-2)


&nbsp;
= 2.0.2.1 =
*Release Date - November 20, 2014*

= Bugfixes =
* Minor JS bug of v2.0.2 fixed


&nbsp;
= 2.0.2 =
*Release Date - November 19, 2014*

= Improvements =
* Taxonomy Settings: you can now rewrite taxonomy slug and permalinks front base

= Bugfixes =
* PRO: fixed a bug preventing repeat saving categories with "Save Changes" button for same set of media files


&nbsp;
= 2.0.1 =
*Release Date - November 16, 2014*

= Bugfixes =
* Front-end: scripts conflict fixed, update if EML breaks your front-end features



&nbsp;
= 2.0 =
*Release Date - November 15, 2014*

= New =
* [PRO vesrion](http://wpuxsolutions.com/plugins/enhanced-media-library/) with long-awaited bulk edit feature is finally released!

= Improvements =
* Media Popup: Filters reset automatically as soon as new media files upload process started
* Media Popup: Selection resets automatically as soon as filter is changed
* Media Popup: WordPress 4.0 date filter added
* Compatibility: general compatibility with other plugins improved, please [let me know](http://wpuxsolutions.com/support/create-new-ticket/) if you have any issue with EML and other plugins

= Bugfixes =
* Media Popup: No delay or glitches anymore when checking media taxonomy checkboxes [Support Request](https://wordpress.org/support/topic/any-way-to-bulk-edit-images/page/2#post-6051963)
* Media Popup: Fixed the bug with non-hierarchical taxonomies (accidentally, only in 1.1.2)
* Media Popup: Filters added to custom posts media popup
* Media Trash: Fixed the incorrect work with MEDIA_TRASH (WordPress 4.0)
* Advanced Custom Fields: Fixed the bug with ACF compatibility [Support Request](https://wordpress.org/support/topic/acf-file-field-conflict-with-eml) and some other minor bugs



&nbsp;
= 1.1.2 =

= Improvements =
* Wordpress 4.0 compatibility ensured


&nbsp;
= 1.1.1 =

= Improvements =
* Filters added for Appearance -> Header and Appearance -> Background [Support Request](https://wordpress.org/support/topic/missing-category-filter-on-media-select-window)

= Bugfixes =
* Fixed EML 1.1 bug with disappearing widgets on Appearance -> Customize [Support Request](http://wordpress.org/support/topic/customize-missing-widgets)
* Fixed EML 1.1 bug with disappearing scrollbar [Support Request](http://wordpress.org/support/topic/scroll-bar-disappeared-in-media-window)


&nbsp;
= 1.1 =

= Improvements =
* Filters added to /wp-admin/customize.php page [Support Request](https://wordpress.org/support/topic/missing-category-filter-on-media-select-window)
* Reconsidered the mechanism of checkboxes' checking in Media Uploader for more stable operation [Support Request](https://wordpress.org/support/topic/instability-in-the-media-insertion-panel)
* Media Uploader filters now work without page refreshing when you change category for you images

= Bugfixes =
* Fixed "Uploads not showing" issue [Support Request](http://wordpress.org/support/topic/uploads-not-showing)
* Reconsidered CSS for filters area [Support Request](http://wordpress.org/support/topic/missing-search-box)
* Fixed CSS and JS files wrong path definitions [Support Request](http://wordpress.org/support/topic/little-bug-2)


&nbsp;
= 1.0.5 =

= Bugfixes =
* Fixed disappearing filter in Media Uploader [Support Request](https://wordpress.org/support/topic/any-chance-of-adding-a-drop-down-in-the-insert-media-screen)
* Added WP 3.9 compatibility [Support Request](https://wordpress.org/support/topic/great-plugin-but-breaks-the-new-add-media-in-39)


&nbsp;
= 1.0.4 =

= Bugfixes =
* Fixed filter mechanism in Media Library [Support Request](http://wordpress.org/support/topic/filter-in-media-not-working-properly)
* Fixed the bug with saving of assigned post categories and tags in Media Uploader


&nbsp;
= 1.0.3 =

= Improvements =
* Better term sorting in Media Uploader
* Minor code improvements

= Bugfixes =
* Fixed the bug with sorting of post categories and tags assigned to Media Library


&nbsp;
= 1.0.2 =

= Bugfixes =
* Fixed assigned non-media taxonomies archive page [Support Request](http://wordpress.org/support/topic/plugin-woocommerce-products-stopped-displaying)


&nbsp;
= 1.0.1 =

= Bugfixes =
* Media Uploader filter now shows nested terms.
* Media Uploader filter now works correctly with multiple taxonomies.


&nbsp;
= 1.0 =

= New =
* Enhanced Media Library initial release.
