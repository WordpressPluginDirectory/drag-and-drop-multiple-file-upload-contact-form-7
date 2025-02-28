=== Drag and Drop Multiple File Upload for Contact Form 7 ===
Contributors: glenwpcoder, yordansoares
Donate link : http://codedropz.com/donation
Tags: drag and drop, contact form 7, ajax uploader, multiple file, upload
Requires at least: 3.0.1
Tested up to: 6.7
Stable tag: 1.3.8.6
Requires PHP: 5.2.4
License: GPLv2 or later
License URI: https://www.gnu.org/licenses/gpl-2.0.html

This simple plugin create Drag & Drop or choose Multiple File upload in your Confact Form 7 Forms.

== Description ==

**Drag and Drop Multiple File Upload** is a simple, straightforward WordPress plugin extension for Contact Form 7, which allows the user to upload multiple files using the **drag-and-drop** feature or the common browse-file of your webform.

Drag and Drop Multiple File Upload for Contact Form 7 is an independent plugin, not affiliated with or endorsed by the developers of Contact Form 7.

Here's a little [DEMO](http://codedropz.com/contact).

### Features

* File Type Validation
* File Size Validation
* Ajax Uploader
* Limit number of files Upload.
* Limit files size for each field
* Can specify custom file types or extension
* Manage Text and Error message in admin settings
* Drag & Drop or Browse File - Multiple Upload
* Support Multiple Drag and Drop in One Form.
* Able to delete uploaded file before being sent
* Send files as **email attachment** or as a **links**. *(see note below)*
* Support multiple languages
* Mobile Responsive
* Cool Progress Bar
* Compatible with any browser

**PLUGIN GUIDE - FREE VERSION**

[youtube https://www.youtube.com/watch?v=DvuvmzIImYo]

**Note:** On Free version, all uploaded files moves to a temporary folder *("/wp-content/uploads/wp_dndcf7_uploads")* then attaches the file to the mail and sends it. After that **"Drag & Drop File Upload"** removes the file from the temporary folder **1 hour** after the submission. *( same process with the default **"file"** upload of Contact Form 7 - [See here](https://contactform7.com/file-uploading-and-attachment/#How-your-uploaded-files-are-managed) )*

To **adjust** or **disable** the auto-deletion feature, we suggest upgrading to the **PRO version** for more options *(see below)*.

### ⭐ Premium Features ⭐

Check out the available features in the **PRO version**.

* **Image Preview** - Show Thumbnail for images
* Adjust **Auto Deletion** of Files - After Form Submission
  - *(1 hour, 4 hours, 8 hours , days, months etc)*
* Zip Files ( Compressed File )
* Save Files to **"Wordpress Media Library"**
* Change Wordpress Upload Directory
* Change **Upload Folder** To:
  - Contact Form 7 - Fields
  - Generated Date & Time - Timestamp
  - Random Folder
  - By User - Required Login
  - Custom Folder
  - Dynamic Folder - *user (name, id), post (id, slug), cf7 fields*
* Send as Individual Email Attachments, Zip Archive, or Links"
* Chunks Upload *( Break large files into smaller Chunks )*
  - Capable of uploading large files.
* set a Max Total Size *( of all Uploaded Files )*
* Parallel Upload *(No. of files that can be uploaded simultaneously)*
* Change **Filename Pattern** ({filename}, {cf7-field-name}, {ip_address}, {random}, {post_id}, {post_slug}, etc.)
* **New** - Color Options (File Size, Progress Bar, Filename, etc.)
* **New** - Disabled the Button to Prevent Duplicate Submissions"
* **New** - Image preview on email
* **New** - File Remote Storage *(OneDrive, Google Drive, Amazon S3, FTP, Dropbox)*
* **New** - Save **Form Entries** in the Admin
* **New** - Select "Dark" or "Light" Theme
* **New** - Validate Image Sizes (Width & Height)
* Able Resize Image (ie: 800x800) - **Standard** Version Only
* Automatically Optimizing Images (**Standard** Version Only)
* Enhanced Security (Updated Regularly)
* Code Optimization and Improved Performance

**Pro version** is also compatible with:

* Contact Form 7 Add-on – Arshid
* Database for Contact Form 7- Ninja
* Advanced Contact form 7 DB – Vsourz Digital

You can get [PRO Version here](https://www.codedropz.com/purchase-plugin/)!

**PRO VERSION - PLUGIN OVERVIEW**

[youtube https://youtu.be/PoQA4KmIETA?si=udM-70n6l4lsQAfp]

### Other Plugin You May Like

* [Drag & Drop Multiple File Upload - WPForms](https://www.codedropz.com/drag-drop-file-uploader-wpforms/)
An extension for **WPForms** - Transform your simple file upload into beautiful **"Drag & Drop Multiple File Upload"**.

* [Drag & Drop Multiple File Upload - WooCommerce](https://wordpress.org/plugins/drag-and-drop-multiple-file-upload-for-woocommerce/)
An extension for **WooCommerce** - Transform your simple file upload into beautiful **"Drag & Drop Multiple File Upload"**.

== Frequently Asked Questions ==

= How can I send feedback or get help with a bug? =

For any bug reports go to <a href="https://wordpress.org/support/plugin/drag-and-drop-multiple-file-upload-contact-form-7">Support</a> page.

= How can I limit file size? =

To limit file size in `multiple file upload` field generator under Contact Form 7, there's a field `File size limit (bytes)`.

You can also manually add limit parameter in existing [mfile] tag.

Example: *[mfile upload-file-433 limit:20971520]* - This limit the user to upload upto 20MB only.

Please take note it should be `Bytes` you may use any converter just Google (MB to Bytes converter) default of this plugin is 5MB(5242880 Bytes).

= How can I limit the number of files in my Upload? =

You can limit the number of files in your file upload by adding this parameter `max-file:3` to your shortcode :

Example: *[mfile upload-file-344 max-file:3]* - this option will limit the user to upload only 3 files.

= How can I Add or Limit file types =

You can add or change file types in cf7 Form-tag Generator Options by adding `jpeg|png|jpg|gif` in `Acceptable file types field`.

Example : *[mfile upload-file-433 filetypes:jpeg|png|jpg|gif]*

= How can I change text in Drag and Drop Uploading area? =

You can change text `Drag & Drop Files Here or Browse Files` text in Wordpress Admin menu under `Contact` > `Drag & Drop Upload`.

= How to Display Links in an Email =

Some email servers have limitations on file attachment sizes (e.g., Google allows a maximum of 20-25 MB). Attaching large files to emails can be problematic. Consider using this option to display links in the email instead of attaching the files.

Go to WP Admin `Contact -> Drag & Drop Upload` settings then check "Send Attachment as links?" option.

To manage mail template, go to Contact Forms edit specific form and Select `Mail` tab. In `Message Body` add generated code from [mfile]. ( Example Below )

Message Body : [your-message]

File Links 1 : [upload-file-754]
File Links2 : [upload-file-755]

Note : No need to add in `File Attachments` field.

See [Video Demonstration](https://www.youtube.com/watch?v=DvuvmzIImYo&t=232s)

= How to Attach Files to an Email =

1. In order to attach files to email you will need to check and make sure **"send as file(s) as links"** option is unchecked.
2. Go to Wordpress admin menu "Contact -> Edit {specific_form}" click or hover the cf7 form you want to edit.
3. In **"Edit Contact Form"** page click "Mail" tab and in the bottom you will see **"File attachments"** field, on this field add your upload field name (ie: **[upload-file-xxx]**), you will find the upload name in **"Form"** tab generated from `[mfile]` shortcode.
4. If attaching multiple files from a different file upload just add all the upload fields name. (see example below)
File attachments: `[upload-file-111] [upload-file-222]`

See [Video Demonstration](https://www.youtube.com/watch?v=DvuvmzIImYo&t=113s)

== Installation ==

To install this plugin see below:

1. Upload the plugin files to the `/wp-content/plugins/drag-and-drop-multiple-file-upload-contact-form-7.zip` directory, or install the plugin through the WordPress plugins screen directly.
2. Activate the plugin through the 'Plugins' screen in WordPress
3. Go to "Contact > Drag & Drop Upload" for the settings.
4. See [Tutorial](https://www.youtube.com/watch?v=DvuvmzIImYo)

== Screenshots ==

1. Generate Upload Field - Admin
2. Form Field Settings - Admin
3. Uploader Settings - Admin
4. Email Attachment- Gmail
5. Email Attachment As links - Gmail
6. Multiple Drag and Drop Fields - Front
7. Remote Storage - Pro Features

== Changelog ==

= 1.3.8.6 =
- Fixes - Security Updates (fixed Vulnerability issue reported by Wordfence - CVE ID:CVE-2024-12267)
- Bug Fix - Fixed bug [Support Link](https://wordpress.org/support/topic/argument-1-value-must-be-of-type-countablearray-string-given/)
- Improvement - Added a random directory for each user/guest uploads to prevent file deletion across folders (related to item # 1)

= 1.3.8.5 =
- Hot fix ( Showing critical error on Php 7.3 and Up )
- Improvement - Improved I18N (Thanks to @alexclassroom)[Support Link](https://wordpress.org/support/topic/improve-i18n-issues-based-on-1-3-8-4/)

= 1.3.8.4 =
- Added Compatibility on Contact Form 7 6.0.
- Wordpress 6.7 Compatibility check.

= 1.3.8.3 =
- Bug - Fixed "send file(s) as links" option not creating year/month folder structure.

= 1.3.8.2 =
- Fixes - Show query error using Query Monitor plugin [Here](https://wordpress.org/support/topic/php-error-pops-up-via-query-monitor/)
- Added - JS/PHP hooks after successful upload [Here](https://wordpress.org/support/topic/javascript-jquery-event-to-trigger-successful-uploads/)
- Tweak - Move error message above files upload [Here](https://wordpress.org/support/topic/is-it-possible-to-move-the-error-message-location/)
- Fixes - Minor fixes and improvements

= 1.3.8.1 =
- Quick Fix - Unable to uncheck "Send file(s) as links" option.

= 1.3.8.0 =
- Quick fix to prevent auto-deletion if the "Don't delete files" setting was overridden by recent updates.

= 1.3.7.9 =
- Bug - Added back the "Don't delete files" option.
- Optimized -  Optimized plugin settings by saving them as an array instead of retrieving individual settings from the wp_options table.
- Compatibility check on latest version of Contact Form 7 5.9.5.

= 1.3.7.8 =
- Added "index.php" file to plugin upload directories for security enhancement, especially for servers like Nginx that do not support .htaccess files. This prevents unauthorized access to files. (Thanks to @Wordfence team for reporting the issue)
- New - Added an option in the admin "Unique Filename" to randomize or generate unique filename.

= 1.3.7.7 =
- Fixes - js/css enabled as default 'dnd_cf7_load_on_cf7_page' filter
- Fixes - Remove javascript:void and replaced with '#' on browse and delete for SEO purposes (JS)

= 1.3.7.6 =
- Fixes - Removed inline css and use proper enqueue (https://wordpress.org/support/topic/html-validation-error-21/)
- Minor bug fixes and improvements

= 1.3.7.5 =
- Fixes - Fixed JS error for custom button type submit.

= 1.3.7.4 =
- Fixes - Security Updates "Unauthenticated Arbitrary File Upload" (Thanks to @István from Wordfence)

= 1.3.7.3 =
- New - Added Chinese (Taiwan) Translation (Thanks to: Alex Lion)
- Fixes - Improve I18N issues [Reported Here](https://wordpress.org/support/topic/improve-i18n-issues-based-on-1-3-7-2/)
- Bug - Remove required error message after user uploaded successfully (JS) [Topic](https://wordpress.org/support/topic/error-message-not-removed/)
- Bug - Clear or reset on multiple form after send (JS) [Topic](https://wordpress.org/support/topic/images-still-in-form-after-send/)
- Fixes - Fixed error console when there's no upload field in the form (JS)

= 1.3.7.2 =
- Bug - Minor JS fixes ( Max limit validation )

= 1.3.7.1 =
- Minor fixes

= 1.3.7.0 =
- Tested on Wordpress 6.3
- Added new option in "Contact -> Drag & Drop Upload" to use jQuery or Native Javascript
- Optimized javascript into 1 file
- New - Transitioning from jQuery to Native Javascript

= 1.3.6.9 =
- Fixes - Quick fix ( Error: Call to a member function id() on null )

= 1.3.6.8 =
- Fixes - Added alternative solution for nonce

= 1.3.6.7 =
- Fixes - for Mime Type validation

= 1.3.6.6 =
- Fixes - Security Fix (CSRF)
- Added - Added security nonce on ajax request for upload and delete

= 1.3.6.5 =
- Fixed - security issue ("Unauthenticated File upload Size limit bypass") thanks to Sanjay Das from "Payatu Security Consulting "
- Added fixes so it should get the size limit on the cf7/admin settings instead of the post request.

= 1.3.6.4 =
- Tested on latest version of wordpress 6.0.
- Added Compatibility on Contact Form 7 version 5.6.

= 1.3.6.3 =
- Fixed - Security issues (Cross-Site Scripting through SVG files via remote upload)
- New - Filter `dnd_cf7_data_options` to manualy change the browse text and label text.

= 1.3.6.2 =
- Added - Add settings link in the plugin page
- Fixed - Long text/heading is hidden on the container
- Fixed - Min file validation
- Bug - Removed "accept" data attributes in mobile devices

= 1.3.6.1 =
- Fixed - Unable to delete if errors will show
- Added “span” & “div” on heading tag option
- Add spam filtering fixes
- Added “Disable Auto Delete” option.

= 1.3.5.9 =
- Add accept types data attributes [See Here](https://wordpress.org/support/topic/the-user-sees-only-a-certain-type-of-files/)

= 1.3.5.8 =
- Fixed German translation (https://wordpress.org/support/topic/german-translation-wrong/)
- Fixes - Bug on file deletion (Reported here - https://wordpress.org/support/topic/deleting-files-not-yet-uploaded-is-breaking/)
- Change delete icon instead of using an iconmoon.
- Minor fixes & Improvement

= 1.3.5.7 =
   - Bug - Fixed validation issue when "CF7 Conditional Fields" plugin is active.

= 1.3.5.6 =
   - New - option to change upload heading tag from h1-h6
   - Change text-domain to actual plugin slug for plugin internationalization.
   - Fixed validation error message for multiple groups. (compatible with CF7 - Conditional Fields)

= 1.3.5.5.1 =
* Bug - Fixed Contact Form 7 error notice
   - PHP Deprecated: id property of a WPCF7_ContactForm object is no longer accessible.
   - Reported here - https://wordpress.org/support/topic/bug-notice-id-not-accessible

= 1.3.5.5 =
* Fixed - Vulnerability (Thanks to @Sysdream Labs team )
   - Removed "supported type" in POST request so other users cannot override through remote access.
   - The issue was, user able to bypass and upload ".phar & .phpt" file extension by modifying "suported type"
   - Those extensions are enabled by default on a fresh PHP/Apache2 installation.
* Improved - Security (file types condition are based on specified in the admin)

= 1.3.5.4 =
* Added - Russian translation (Thanks to "Dan Uchvatoff ")
* Fixed - File counter "of" not translatable.

= 1.3.5.3 =
* Fixed - PHP Fatal error on server not supporting mb_check_encoding.
* Fixed - Fatal error: Uncaught Error: Call to a member function scan_form_tags()
  - When "Accept PayPal Payments using Contact Form 7" installed.

= 1.3.5.2 =
* Added - Improved sercurity ( Limit the user input to a file name and ignore injected path names )
* Modified - Email links ( display only the filename )

= 1.3.5.1 =
* Bug - Quick Fix ( Unable to submit form when acceptance field is set  )
   - Issue if "additional settings" section added  this line: acceptance_as_validation: on

= 1.3.5 =
* Fixed - nonce issues when using Cache plugins.
* Fixed - German Translation for ( Drag & Drop File Upload ) text.
* Fixed - Submit button ( enable/disable ) when acceptance checkbox is added.
* Modified - File Upload error message  ( display error code )

= 1.3.4 =
* Fixed - Removed uploaded files when item Inbound Messages "Permanently Deleted".
* Added -  Counter of how many files are uploaded ( ie: 4 of 10 )
* New - Features allow to set Minimum File Upload.
- ie : minimum upload:2, max upload:10 = [mfile* upload-file-669 min-file:2 max-file:10]
* New - Added .htaccess file inside "wp_dndcf7_uploads" upload directory. ( prevent from direct access )
- Options: -Indexes \n <Files *.php> \n deny from all \n </Files>
* Fixed - File Attachments bug ( Issues on additional mail when (file attachment) is removed still send the file )

= 1.3.3.3.2 =
* Bugs - Fixed unable to submit form ( 500 Internal Server Error in response )

= 1.3.3.3.1 =
* Fixes - Minor updates (packed the wrong file)

= 1.3.3.3 =
* Fixed  - Security Issues ( Unrestricted File Upload to Remote Code Execution - Thanks to @Austin  )
  -  Able bypass and upload file (remotely) by renaming to ie: shell.php% and modified supported_type to `jpg|png|php%`
  - Solution : Added more security, check/validate file type and created new function 'dnd_cf7_validate_type' to determine if file name extension is valid or not.
* New - Make 'deleting...' and 'remove' text translatable ( compatible using WPML String Translation ).

= 1.3.3.2 =
* Fixed  - PHP warning reported [here](https://wordpress.org/support/topic/php-warning-count-parameter-must-be-an-array-2/)

= 1.3.3.1 =
* Improved Security - ( Check valid filename & extensions, sanitations, Secured File deletions )
* New - Allowed non ASCII file name
* Improved styling on Progress Bar
* Fixed - Conflict with WooCommerce Geo Location

= 1.3.3 =
* SECURITY UPDATES ( issues reported by : Robert L Mathews )
- The issues inside `dnd_codedropz_upload_delete` function, that will execute any POST remotely.
* Fixed - To accept russian, hebrew Filename
* Modify Javascript `dnd-upload-cf7.js` attach the function to window so it can be available to call.
* Added - Responsive style for `Drag & Drop` text on mobile devices.
* Minimum Features - Coming Soon

= 1.3.2 =
* Fixed - Sanitized Admin Option Fields - For Security Reason
* Added - Filter for `wpcf7_posted_data` from CF7 to get the full link of the file.

= 1.3.1 =
* Fixed - Browser Compatibility ( Error Uploading files in Edge, Safari and Internet Explorer )
* Improved - Removed error text if there are muliple error ( File upload validation )

= 1.3.0 =
* Fixed - Multiple Drag & Drop fields in one form ( Validation Issues - Max File not working correctly )
* Added - Added "deleted..." status when removing file.
  - So that the user know that file deletion is in progress...
* Fixed - Responsive issues on Mobile < 767px screen.
* Added - Added '/wpcf7-files' directory inside '/wp_dndcf7_uploads' to temporary store files instead of relying contact form 7.
* Added - Auto delete files inside '/wpcf7-files' dir 1 hour(3200 seconds) after submission.
  - It was a problem with contact form 7 before that files only last 60 seconds and it will automatically deleted.
* Improved - Optimized and Improved Php Code & Javascript structure and functionalities. ( removed redundant code, removed spaces, etc )
* Added - Links going to Pro Version.

= 1.2.6.0 =
* Fixed - Allow to upload file with the same filename.
* Fixed - Can't upload image after deleting (https://wordpress.org/support/topic/cant-upload-image-after-deleting-it/)
* Fixed - Max-file issue (https://wordpress.org/support/topic/max-file-issue/)
* Added - a note message when file reached the max-file Limit ( "To inform user that some of the files are not uploaded" ).
* Added - Better Ajax deletion ( Remove files from the server - Only if `Send As Attachment` is checked )
* Optimized - Form send loading time has been optimized ( Improved loading time for large attachment )
* Fixed - Bug reported by @palychwp " `remove file still send sends with the form` (https://wordpress.org/support/topic/file-uploading-is-working-incorrect/)
* Added - Validate File/Attachment first before the upload start ("some says it's frustating :)")
  - (PHP or Server side validation still there for security and better validation)
* Improved file counting via `LocalStorage` instead of Global variable.

= 1.2.5.0 =
* Fixed - Please Update to 1.2.5.0 to fixed disable button issue.

= 1.2.5 =
* Fixed - Improved ( Disable button while upload is on progress )
* Fixes - Validate file size limit before uploading the file ( https://wordpress.org/support/topic/file-uploading-is-working-incorrect/ )

= 1.2.4 =
* Added - Support WPML using .po and .mo files
* Added - Added to support multilingual ( using Poedit )
* Fixed - Prevent attachment from sending to Mail(2) if field attachment is not set. (https://wordpress.org/support/topic/problem-with-2th-mail-attachment-2/)
* Added - Disable 'submit' button while upload is on progress...

= 1.2.3 =
* Added - Multiple Drag and Drop fields in a form
* Added - Options in admin for error message
* Added - Option that allow user to send attachment as links
* Added - Added new folder name `wp_dndcf7_uploads` to separate files from wpcf7_uploads ( When option 'Send Attachment as links?' is check ).

= 1.2.2 =
* Add - Create admin settings where you can manage or change text in your uploading area. It's under 'contacts' > 'Drag and Drop'.
* New - Empty or Clear attachment file when Contact Form successfully send.
* Fixes - Fixed remove item bugs when file is greater than file limit.
* Fixes - Changed 'icon-moon' fonts to avoid conflict with the other themes.
* New - Added text domain for language translations.

= 1.2.2 =
* Issue - fixed bug when file is not required(*).
* Issue - fixed error on 'wpcf7_mail_components' components hooks when there's no file.

= 1.2.1 =
* Issue - fixed bug when file is not required(*).
* Issue - fixed error on 'wpcf7_mail_components' components hooks when there's no file.

= 1.2 =
- Add admin option to limit the number of files. (Maximum File Upload Limit)

= 1.1 =
- This version fixes on user drop validation.
- Optimized Javascript File

= 1.0 =
* Initial Release

== Upgrade Notice ==

= 1.2.3 =
This version fixed minor issues/bugs and add multiple drag and drop fields in a form.

= 1.2.1 =
This version fixed minor issues and bugs.

= 1.2.2 =
Added some useful features.

= 1.2.4 =
Added new features and fixes.

== Donations ==

Would you like to support the advancement of this plugin? [Donate](http://codedropz.com/donation)