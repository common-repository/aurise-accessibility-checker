=== AuRise Accessibility Checker ===
Contributors: tessawatkinsllc
Donate link: https://just1voice.com/donate/
Tags: accessible, a11y, wcag, ada, Section 508
Tested up to: 6.6
Stable tag: 1.0.2
Requires PHP: 5.4
License: GPLv3 or higher
License URI: https://www.gnu.org/licenses/gpl-3.0.html

Visualize how your site works with assistive technologies to improve accessibility using tota11y.

== Description ==

The internet is a wonderful place but not all websites are accessible to everyone. This plugin aims to help WordPress website owners test, check, and QA their websites for improvements on making them accessible.

= What does it do? =

This plugin adds [tota11y®](https://blog.khanacademy.org/tota11y-an-accessibility-visualization-toolkit/), an accessibility visualization toolkit, to the frontend of your website for site admins so you can easily see it marked up with annotations on where your site fails and succeeds in addressing accessibility.

= What is Tested? =

**Headings**

Highlights headings (`<h1>`, `<h2>`, etc.) and order violations

**Contrast**

Labels elements with insufficient Contrast

**Link Text**

Identifies links that may be confusing when read by a screen reader

**Labels**

Identifies inputs with missing labels

**Image alt-text**

Annotates images without alt text

**Landmarks**

Labels all ARIA landmarks

**Screen Reader Wand (Experimental)**

Hover over elements to view them as a screen reader would

== Installation ==

There are three (3) ways to install my plugin: automatically, upload, or manually.

= Install Method 1: Automatic Installation =

Automatic installation is the easiest option as WordPress handles the file transfers itself and you don't need to leave your web browser.

1. Log in to your WordPress dashboard.
1. Navigate to **Plugins > Add New**.
1. Where it says "Keyword" in a dropdown, change it to "Author"
1. In the search form, type `TessaWatkinsLLC` (results may begin populating as you type but my plugins will only show when the full name is there)
1. Once you've found my plugin in the search results that appear, click the **Install Now** button and wait for the installation process to complete.
1. Once the installation process is completed, click the **Activate** button to activate it.

= Install Method 2: Upload via WordPress Admin =

This method involves is a little more involved. You don't need to leave your web browser, but you'll need to download and then upload the files yourself.

1. [Download my plugin](https://wordpress.org/plugins/aurise-accessibility-checker/) from WordPress.org; it will be in the form of a zip file.
1. Log in to your WordPress dashboard.
1. Navigate to **Plugins > Add New**.
1. Click the **Upload Plugin** button at the top of the screen.
1. Select the zip file from your local file system that was downloaded in step 1.
1. Click the **Install Now** button and wait for the installation process to complete.
1. Once the installation process is completed, click the **Activate** button to activate it.

= Install Method 3: Manual Installation =

This method is the most involved as it requires you to be familiar with the process of transferring files using an SFTP client.

1. [Download my plugin](https://wordpress.org/plugins/aurise-accessibility-checker/) from WordPress.org; it will be in the form of a zip file.
1. Unzip the contents; you should have a single folder named `aurise-accessibility-checker`.
1. Connect to your WordPress server with your favorite SFTP client.
1. Copy the folder from step 2 to the `/wp-content/plugins/` folder in your WordPress directory. Once the folder and all of its files are there, installation is complete.
1. Now log in to your WordPress dashboard.
1. Navigate to **Plugins > Installed Plugins**. You should now see my plugin in your list.
1. Click the **Activate** button under my plugin to activate it.

== Screenshots ==

1. Close-up of the tota11y widget
2. Screenshot of author's homepage with a red arrow drawn over to point to the widget fixed to the bottom left of the browser window
3. Screenshot of the author's homepage with the tota11y widget menu opened showing the available features to test: headings, contrast, link text, labels, image alt-text, landmarks and screen reader wand (experimental)
4. Screenshot of the author's homepage with the headings feature enabled. The screenshot is annotated with a red circle over the headings option in the menu showing it is checked and red arrows pointing to the headings summary along with the display of headings on the page itself that match the indented list in the summary tab.
5. Screenshot of the author's homepage with the contrast feature enabled. The screenshot is annotated with a red circle over the contrast option in the menu showing it is checked and red arrows pointing to the contrast ratio calcuations that appear around various elements. A calcuation in green shows that it passes validation while one in red shows it fails.
6. Screenshot of the author's homepage with the landmarks feature enabled. The screenshot is annotated with a red circle over the landmarks option in the menu showing it is checked and red circles around the yellow labels displaying landmarks discovered on the webpage.
7. An animated GIF image showing the author's homepage with the screen reader wand enabled. The looping GIF image shows a cursor moving around the page, showing how a blue box highlights various elements on the page while it also displays the screen-reader friendly text from that element in the bottom right box.
8. Screenshot of the settings screen in the WordPress backend. It shows the default settings where "Enabled" is turned on, "Allowed User Roles" is set to "administrator" and "Debug Mode" is turned off.

== Frequently Asked Questions ==

= How do I use it? =

Simply install/activate the plugin and view the frontend of your WordPress website! The widget will appear as a small, black block with a pair of white sunglasses fixed to the bottom-left of your browser. Click on the widget to open its menu for the different types of tools you can use.

= Who can see the testing widget? =

By default, the widget will only appear for WordPress administrators, so your site's viewers will not see the widget.

= How does it work? =

This plugin uses an accessibility visualization toolkit called [tota11y](https://blog.khanacademy.org/tota11y-an-accessibility-visualization-toolkit/).

= Can I turn it off if I don't have access to the plugin page? =

Yes! You can turn it on or off from the settings screen under **Settings > Accessibility Checker**. It is the first setting labled **Enabled**

= How can I enable this for my editors? =

On the settings screen under **Settings > Accessibility Checker**, you can edit the text field for **Allowed User Roles** to be something like `administrator,editor` to allow users with the editor role to see the widget when it's enabled. This also works for custom user roles too. The default value is set to `administrator` and is inclusive of super admins for multisite installations.

= How can I make it so it's only enabled if `WP_DEBUG` is set to true? =

On the settings screen under **Settings > Accessibility Checker**, simply toggle the setting for **Debug Mode** to on and save your settings.

= Can I set these settings using constant variables in my wp-config.php? =

Yes! Whether you want to force all websites in a multisite installation to use the same settings or easily push settings from one installation to another, you can do so with these constant variables.


    define('AURISE_ACCESSIBILITY_CHECKER_ENABLED', true); // Display the widget for allowed roles
    define('AURISE_ACCESSIBILITY_CHECKER_ALLOWED_ROLES', 'administrator'); // Comma-separated list of user roles allowed to see the widget
    define('AURISE_ACCESSIBILITY_CHECKER_DEBUG_MODE', true); // If true, only show the widget to the allowed user roles when WP_DEBUG is also set to true

= Is this the official tota11y WordPress plugin? =

No, this WordPress plugin is not a product of tota11y or its creators, the Khan Academy. It was developed by an independent and disabled web developer that wants to bring more accessibility to the digital space.

== Upgrade Notice ==

= 1.0.0 =

First release!

== Changelog ==

= 1.0.2 =
**Release Date: August 31, 2024**

* Marked compatible with WordPress core 6.6.
* Updated tota11y's broken link to one that isn't broken.

= 1.0.1 =
**Release Date: April 20, 2024**

* Update: Utilized the new feature to defer load the script in the footer.
* Marked compatible with WordPress core 6.5.

= 1.0.0 =
**Release Date: February 15, 2023**

* First release to the official WordPress plugin repository!