## WordPress

#### Q1. In WordPress, what is the Loop used to do?

- [ ] It displays a single page.
- [ ] It displays posts on an archive.
- [ ] It displays a single post.
- [x] all of these answers

#### Q2. Who owns the trademark for WordPress and WordCamp names and logos?

- [x] WordPress Foundation (The WordPress Foundation owns and oversees the trademarks for the WordPress and WordCamp names and logos.)
- [ ] WordPress.com
- [ ] Matt Mullenweg
- [ ] Automattic

#### Q3. What is the name of the open-source project that serves as a bug tracker and project management tool for WordPress?

- [ ] HackerOne
- [ ] Redmine
- [x] Trac
- [ ] GitHub Issues

#### Q4. The REST API is a simple way to get data in and out of WordPress over HTTP. Applications using the REST API should be written in which programming language?

- [ ] PHP
- [x] any programming language that can make HTTP requests and interpret JSON
- [ ] Java
- [ ] Node.js

#### Q5. How many minutes does it take to install WordPress according to the "Famous X-Minute Installation" instructions on WordPress.org?

- [x] 5
- [ ] 30
- [ ] 15
- [ ] 10

#### Q6. In WordPress, what is true of plugins?

- [ ] Plugins are available in free or premium (paid) versions.
- [ ] Plugins can extend WordPress core functionality.
- [x] all of these answers
- [ ] Plugins add site-specific features.

#### Q7. Akismet is a plugin that comes automatically installed with WordPress. What does it do?

- [ ] It connects your site to Google Analytics.
- [ ] It displays a blog feed from websites similar to yours.
- [x] It protects your site from comment spam.
- [ ] It hardens site security by enforcing strong passwords.

#### Q8. What would you do to improve your site's performance?

- [ ] Only load scripts and styles on pages where they are needed.
- [ ] Minify CSS and JavaScript files.
- [x] all of these answers
- [ ] Use a CDN.

#### Q9. The REST API utilizes which data format?

- [ ] YAML
- [x] JSON
- [ ] TXT
- [ ] XML

#### Q10. What color is the paragraph nested within the div?

```html
<head>
    <style>
        body { color: black; }

        p { color: blue; }

        div { color: green; }

        p { color: red; }
    </style>
</head>
<body>
    <div>
        <p>This is a paragraph inside a div.</p>
    </div>
</body>
</html>
```

- [ ] blue
- [ ] black
- [x] red
- [ ] green

#### Q11. Theme developers can take advantage of the

izer API to give users a way to manipulate basic theme settings. The Customizer API is object-oriented and provides four main objects. What are they?

- [ ] widgets, containers, sections, settings
- [ ] containers, hooks, settings, styles
- [ ] panels, blocks, controls, settings
- [x] panels, sections, controls, settings

#### Q12. Which WordPress setting would you use to make page URLs look like `http://example.com/my-page/` instead of the default `http://example.com/?p=21/?`

- [ ] Writing
- [x] Permalinks
- [ ] Pretty URLs
- [ ] Reading

#### Q13. In WordPress, what is the block editor used for?

- [ ] cropping images in the media library
- [ ] injecting specialized scripts into the content area
- [ ] creating a site layout
- [x] creating and laying out content

#### Q14. Which of the following file types is NOT involved in translating WordPress?

- [ ] .po
- [ ] .pot
- [x] .mot
- [ ] .mo

#### Q15. What is the default priority for an action hook or filter?

- [x] 10
- [ ] 15
- [ ] 0
- [ ] 5

#### Q16. What's the primary difference between template tags prefaced with the **versus get_the**?

- [ ] Template tags prefaced with the \_ don't accept arguments.
- [ ] Template tags prefaced with the \_ can be used directly within a template.
- [x] Template tags prefaced with the \_ display a value. Template tags prefaced with get_the return a value.
- [ ] Template tags prefaced with the \_ return a value. Template tags prefaced with get_the display a value.

#### Q17. WP_Query is the WordPress query class that is used to fetch posts from the database. How would you create a new instance of this class?

- [ ] `$query = new query_posts();`
- [x] `$query = new WP_Query();`
- [ ] `$query = query_posts();`
- [ ] `$query = get_posts();`

#### Q18. What is a user role that is unique to WordPress Multisite?

- [ ] MU Admin
- [ ] Owner
- [x] Super Admin
- [ ] Multisite Master

#### Q19. Within the editor, blocks are rendered as JavaScript. How are blocks rendered on the front end of a site?

- [ ] as plain HTML
- [x] as a React component
- [ ] as JavaScript comments
- [ ] as HTML comments

#### Q20. Which of these is NOT a part of the internationalization and localization process?

- [ ] using a gettext function to wrap translatable strings when writing code
- [ ] installing/using the WordPress Multilingual Plugin
- [ ] using a tool like Poedit to parse source code and extract translatable strings into a POT file
- [x] translators translating the POT file into a PO file, one for each language

#### Q21. The REST API provides public data, which is accessible to any client anonymously, as well as private data available only after authentication. How could you ensure that no one can anonymously access site data via the REST API?

- [ ] Disable the REST API via the site's wp-config.php file.
- [ ] Use the `rest_authentication_errors()` filter along with the `is_user_logged_in()` conditional to limit access to logged in users.
- [ ] Use the `rest_authentication_errors()` filter along with cookie authentication to limit access to logged in users.
- [x] Use the Disable REST API plugin.

#### Q22. Which of these snippets represents a wrapper that calls jQuery safely and doesn't require repetitive use of the word "jQuery"?

- [ ] .

```js
$.ready(function () {
  // do stuff
});
```

- [ ] .

```js
(function ($) {
  // do stuff
})(jQuery);
```

- [x] .

```js
$(function () {
  // do stuff
});
```

- [ ] .

```js
jQuery(function ($) {
  // do stuff
});
```

#### Q23. What is the correct order of parameters for the add_action() function?

- [ ] `add_action( 'example_hook', 'example_function', $accepted_args, $priority )`
- [ ] `add_action( 'example_function', 'example_hook', $priority, $accepted_args )`
- [x] `add_action( 'example_hook', 'example_function', $priority, $accepted_args )`
- [ ] `add_action( 'example_function', 'example_hook', $priority )`

#### Q24. You have a search bar on your site. You would like to use a `<label>` to make the word "Search" visible to screen readers, but you don't want to display the word "Search" on the screen. How can you accomplish this?

- [ ] Assign an ARIA state of "hidden" to the label, like this: `<label state="hidden">Search</label> <input type="text" name="search" id="search" />`
- [x] Use the built-in WordPress CSS class .screen-reader-text to hide the text from screen, like this: `<label class="screen-reader-text">Search</label> <input type="text" name="search" id="search" />`
- [ ] Create a custom CSS class to set a large negative value to the text-indent property to hide the text off screen, like this: `<label class="hide-this">Search</label> <input type="text" name="search" id="search" />`
- [ ] The majority of users do not require a screen reader. Remove the label entirely.

#### Q25. You might see this code in a WordPress plugin. What does it do?

```
if ( ! defined( 'ABSPATH' ) ) {
   die;
}
```

- [ ] This is how WordPress detects a plugin's presence. This ensures that the plugin is running from the /wp-content/plugins/ directory. If it is not, the plugin should not run.
- [ ] This is a way to prevent naming collisions. ABSPATH is the absolute path to the plugin's directory. If ABSPATH is defined by another WordPress plugin with the same directory slug, the plugin should not run.
- [x] This is a security measure. ABSPATH is the absolute path to the WordPress directory. If the file is called directly, ABSPATH will not be defined and therefore the plugin should not run.
- [ ] This is a compatibility checker. ABSPATH is defined in WordPress core. The plugin checks that the minimum version of WordPress needed to support the plugin is installed. If it is not, the plugin should not run.

[Reference](https://stackoverflow.com/questions/43212340/what-is-meant-by-if-defined-abspath)

#### Q26. Which is a best practice for working with WordPress CSS?

- [ ] Use !important next to styles if they don't give you the result you want.
- [ ] Use hyphens in class names.
- [x] Use spaces to indent each property.
- [ ] Avoid CSS shorthand for proper documentation.

#### Q27. WordPress is translated, at least partially, in more than 200 locales. If you wanted to help translate WordPress into other languages, which contributor group would you join?

- [ ] core
- [x] polyglots
- [ ] accessibility
- [ ] documentation

#### Q28. What is the difference between an action and a filter?

- [ ] Actions are used to add custom functions and remove WordPress functions. Filters are used to make strings translatable for localization.
- [x] Actions are used to add or remove code at runtime. Filters are used to modify data before it is either displayed in the browser or saved to the database.
- [ ] Actions are used to assign values to variables at runtime. Filters are used to extract data from actions and display it in the browser.
- [ ] Actions are used to add user-inputted data to the database. Filters are used to validate user-inputted data prior to adding it to the database.

#### Q29. If you activate or update a plugin and it breaks your site so that you cannot manage it via wp-admin, how can you disable the plugin?

- [x] all of these answers
- [ ] Access the WordPress install via WP-CLI. Run the following command: wp plugin deactivate offending-plugin.
- [ ] Access site files via FTP and navigate to /wp-content/plugins/. Delete the folder of the plugin that you would like to disable or simply rename it.
- [ ] Use phpMyAdmin to change the wp_options table's active_plugins option value to a:0:{}.

#### Q30. The WordPress REST API is designed to receive and respond to particular types of requests using basic HTML methods. For example, a request to upload a PHP file into a particular folder on a server might look like the code POST `/folder/_file.php`. Based on this code, what would you call /folder/\_file.php (in REST API terms)?

- [ ] schema
- [ ] route
- [ ] response
- [x] request

#### Q31. Which WP-CLI command would you use to manage the capabilities of a user role?

- [ ] wp admin
- [ ] wp manage
- [ ] wp cap
- [x] wp role

#### Q32. What technique would you use to secure data before rendering it to a user?

- [ ] escape and sanitize
- [ ] validate and escape
- [x] validate and sanitize
- [ ] escape and secure

#### Q33. If your WordPress site is seriously compromised, what is the best course of action to return your site to good health?

- [ ] Determine the date of the attack and restore your site to a backup point prior to that date.
- [x] Hire a third-party service to clean up your site because it is difficult for someone who is not a WordPress security expert to find and remove all traces of an attack.
- [ ] Manually delete suspicious files on the server and delete any database tables that are not core WordPress.
- [ ] Change your hosting password, your WordPress admin password, and your database password.

**Explanation**: It's not the cheapest, but it's the most reliable. Restoring the backup might not help if you have backdoor scripts installed outside of WP directory.

#### Q34. If you wanted to register a custom post type, which hook would you use?

- [x] register_post_type
- [ ] add_meta_box
- [ ] wp_head
- [ ] init

#### Q35. What is the role of a WordPress theme?

- [ ] controls colors, fonts, and page layouts
- [ ] adds accessibility enhancements such as keyboard navigation and skip links
- [ ] ensures a site is mobile responsive
- [x] all of these answers

#### Q36. What is the core mission of WordPress?

- [ ] to make free software
- [x] to democratize publishing and the freedoms that come with open source
- [ ] to make money
- [ ] to encourage blogging

[Reference](https://wordpress.com/about/)

#### Q37. Which of the following is NOT a suggested security improvement for your WordPress website?

- [ ] The site should communicate with WordPress.org.
- [ ] Remove inactive themes.
- [ ] Do not output debug information.
- [x] WordPress updates are accomplished manually only.

**Explanation**: Communicating with WordPress.org is needed for detecting new versions.

#### Q38. How can you add a custom script that needs to run only on the contact page of a site? The slug of the page is contact.

- [ ] Link to the script directly from a template named page-contact.php using the get_header() template tag, like this:

```
get_header( '<script src="/my-script.js"></script>' );
```

- [ ] Use functions.php to conditionally load the script by hooking it to wp_enqueue_scripts(), like this:

```
add_action( 'wp_enqueue_scripts', 'load_scripts' );

function load_scripts() {
    if ( is_page( 'contact' ) ) {
    echo '<script src="/my-script.js"></script>';
    }
}
```

- [ ] Use functions.php to conditionally load the script by hooking it to wp_enqueue_scripts(), like this:

```
add_action( 'wp_enqueue_scripts', 'load_scripts' );
    function load_scripts() {
        if ( is_page( 'contact' ) ) {
        wp_enqueue_script( 'script', get_template_directory_uri() . '/script.js' );
        }
    }
```

- [x] Link to the script directly from a template named page-contact.php, like this:

```
<head>
  <script src="/my-script.js"></script>
</head>
```

#### Q39. Where can you find the official WordPress documentation and usage guide?

- [ ] `support.wordpress.com`
- [ ] `developer.wordpress.com`
- [x] `developer.wordpress.org`
- [ ] `support.wordpress.org`

#### Q40. How would you use CSS to ensure your theme was mobile responsive?

- [ ] Use CSS grid to create responsive layouts.
- [x] Use media queries to add breakpoints for different screen sizes.
- [ ] Use Flexbox to create flexible page layouts.
- [ ] all of these answers

#### Q41. The Block API enables developers to register custom blocks in themes or plugins. How would you register a custom block?

- [ ] Use the registerBlockName() function.
- [ ] Use the createGutenBlock() function.
- [ ] Use a block template.
- [x] Use the registerBlockType() function.

#### Q42. Which software development principle, often used in WordPress, aims to reduce the repetition of code?

- [ ] RRR
- [ ] WET
- [x] DRY
- [ ] KISS

`DRY(Don't Repeat Yourself)`

#### Q43. In a standard template file, how often does the WordPress Loop run?

- [ ] It runs once per post in the database.
- [ ] It runs once.
- [ ] The Loop doesn't run in template files.
- [x] It runs once per fetched post.

#### Q44. Which is NOT a suggested performance improvement for your WordPress website?

- [ ] The site should run the most recent version of WordPress.
- [ ] Remove or inactivate unnecessary plugins.
- [x] UTF8 is supported.
- [ ] Choose a very recent version of PHP.

**Explanation**: New versions usually come with speed improvements. Inactivating plugins improves performance. By exclusion, it's UTF8.

#### Q45. On a regular WordPress install, what is the difference between transients and the object cache?

- [x] Transients are persistent and write to the wp_options. The object cache persists only for the particular page load.
- [ ] Transients are stored in the WordPress database. The object cache is stored on the server where the WordPress install is located.
- [ ] Transients are available for the duration of a user session and apply to all page components. The object cache is available only for scripts.
- [ ] Transients persist only for the particular page load. The object cache is persistent and writes to the wp_options table.

#### Q46. You can harden your WordPress site security by adding `__` to your wp-config.php file?

- [ ] database usernames and passwords
- [x] unique keys and salts
- [ ] accessibility
- [ ] documentation

[Reference](https://www.malcare.com/blog/how-to-secure-your-wordpress-site-with-wp-config-php/)

#### Q47. According to WordPress PHP coding standards for inline comments, how would you write a single-line comment in a PHP document?

- [x] `// This is a single line comment`
- [ ] `/\* _ This is a single line comment._/`
- [ ] `// This is a single line comment.`
- [ ] `<!-- This is a single line comment -->`

#### Q48. If you have pretty permalinks enabled on a WordPress site, the REST API index is exposed by appending what to the end of the site URL? (for example, http://example.com/answer/) Note that the index provides information regarding which routes are available for that particular WordPress install.

- [x] `http://example.com/wp-json/`
- [ ] `http://example.com/wp-admin/`
- [ ] `http://example.com/wp-rest/`
- [ ] `http://example.com/wp-rest-api/`

#### Q49. What is the process of marking the code you write so that it is ready for translation?

- [x] internationalization
- [ ] localization
- [ ] translation
- [ ] using GlotPress

**Explanation**: Localization and translation are synonyms for submitting language-specific translation. GlotPress is just a Wordpress plugin.

#### Q50. In your wp-config.php file, you've added the following line of code. What does it do?

`define( 'DISALLOW_FILE_EDIT', true );`

- [ ] prevents any non-admin user from directly editing theme or plugin files
- [x] disables the theme and plugin editor in the WordPress admin
- [ ] disables the ability to edit core WordPress files from either within the WordPress admin or via direct file access
- [ ] sets read-only permissions on all files in the WordPress install

[More WordPress Security: Disallow File Edit Setting In WordPress](https://www.icontrolwp.com/blog/more-wordpress-security-disallow-file-edit-setting-wordpress/). Setting all files to read-only would make auto-updates impossible.

#### Q51. Which of the following must have underlined links in order to meet WCAG 2.0 accessibility standards?

- [ ] links on images
- [ ] links in user interface controls
- [ ] links in a nav bar
- [x] links in paragraph text

#### Q52. In which of the following ways might you contribute to the WordPress community by testing?

- [ ] user testing
- [x] all of these answers
- [ ] beta testing
- [ ] automated testing

#### Q53. WordPress is an open-source software licensed under the GPL. This means that `__`.

- [ ] derivative works must also be licensed as GPL
- [x] all of these answers
- [ ] the software is free to use
- [ ] the software is free to modify

#### Q54. Review the HTML on line 1. The goal of the PHP on line 2 is to extract the field value and assign it to a variable prior to inserting into the database. What is wrong with this PHP code?

```
<input type="text" id="title" name="title" />
$title = $_POST[ 'title' ];
```

- [ ] The code sample does not use the GET method. It should be wrapped in the `get_post_field()` function and look like this `$title = get_post_field( $GET[ 'title' ] );`
- [x] The code sample does not sanitize the form data. It should use the `sanitize_text_field()` function and look like this: `$title = sanitize_text_field( $_POST[ 'title' ] );`
- [ ] There is no error. The code follows WordPress best practices.
- [ ] The code sample does not allow for translation. It should use a translation function and look like this: `$title = __( $_POST[ 'title' ];`

[Ref](https://hazimhassan.com/linkedin-wordpress-assessment-answers-2021/)

#### Q55. Which of these CSS classs naming convention is correct according to WordPress CSS Coding Standards?

- [x] `.selector-name`
- [ ] `.selector_name`
- [ ] `.selectorName`
- [ ] `div.selector_name`

[Reference - Avoid Underscores](https://developer.wordpress.org/coding-standards/wordpress-coding-standards/css/#selectors)

#### Q56. Which folder in a WordPress install is not affected by an automatic WordPress update?

- [ ] `/wp-admin`
- [ ] `root`
- [x] `/wp-content`
- [ ] `/wp-includes`

#### Q57. What are transients?

- [ ] short database queries
- [x] a way to cache information
- [ ] plugins used for quick debugging
- [ ] post draft stored in the database

**Explanation**: [Transients](https://developer.wordpress.org/apis/handbook/transients/)

#### Q58. If you wanted to debug some JavaScript, which method would you use to display data in your browser console?

- [ ] `windows.alert()`
- [x] `console.log()`
- [ ] `document.write()`
- [ ] `innerHTML`

#### Q59. On a webpage, there are frequently navigation links, a search bar, or other elements that appear before the main content. For keyborad and screen reader users, it can be frustrating to get to the main content of a page because they have to tab through all these elements on every new page load. What can you add to a site to fix this?

- [x] collapsible menus
- [ ] infinite scroll
- [ ] skip links
- [ ] tabbed navigation

#### Q60. What user role would you assign to someone so they can write and publish only their posts and no one else's?

- [ ] Contributor
- [x] Author
- [ ] Editor
- [ ] Subscriber

**Explanation**: [Summary of Roles](https://wordpress.org/support/article/roles-and-capabilities/#summary-of-roles)

#### Q61. When should you edit core WordPress files?

- [ ] when there is no plugin available to make a customization you need
- [ ] when you need to add a custom page template
- [ ] when you need to add a custom script to the header or footer of every page in a site
- [x] You should never edit WordPress core.

**Explanation**: It is not recommended to change WordPress core files other than wp-config.php. [Editing Files Offline](https://wordpress.org/support/article/editing-files/#editing-files-offline)

#### Q62. Which Wordpress conditional would you use to determine if you were on a single page?

- [ ] is_archive()
- [ ] is_page()
- [ ] is_page_template()
- [x] is_single()

[Reference](https://developer.wordpress.org/reference/functions/is_single/)

#### Q63. Wordpress core and many plugins store data in the database in a special format as represented by the sample below. What format is this called?

`a:2:{i:0;s:27:"ari-adminer/ari-adminer.php";i:1;s:30:"atomic-blocks/atomicblocks.php";}`

- [ ] value
- [x] serialized data
- [ ] PHP array
- [ ] text array

[Reference](https://wpengine.com/support/wordpress-serialized-data/)

#### Q64. What is this code sample an example of?

```
<?php
if ( have_posts() ) : while ( have_posts() ) : the_post();
        the_content();
endwhile;
else :
        _e( 'Sorry, no posts matched your criteria.', 'textdomain' );
endif;
```

- [ ] custom query
- [ ] template tags
- [x] the Loop
- [ ] nested loop

#### Q65. Which of these are the minimum files required to make a child theme?

- [ ] index.php functions.php
- [ ] index.php style.css script.js
- [ ] functions.php style.css script.js
- [x] functions.php style.css

[Reference](https://kinsta.com/blog/wordpress-child-theme/)

#### Q66. In the WordPress template hierarchy, which file could not be used to display an archive?

- [ ] `archive.php`
- [x] `index.php`
- [ ] `page.php`
- [ ] `category.php`

[Reference](https://developer.wordpress.org/themes/basics/template-hierarchy/)

#### Q67. Why can't you modify the query in a template page?

- [ ] The query can only be run inside the Loop.
- [x] You can modify the query in a template page if you use `pre_get_posts()`.
- [ ] According to WordPress best practices, the query should only be modified in `functions.php`.
- [ ] Due to execution order, the query has already run by the time a template is loaded.

[Reference](https://webcraft.tools/how-to-modify-the-main-wordpress-query/)

#### Q68. For the majority of modern themes, what is the standard method used to customize various details of site appearance and features, such as changing the site description or adding a logo and favicons?

- [ ] WordPress settings
- [x] Customizer
- [ ] wp-config.php
- [ ] Theme settings

[Reference](https://wordpress.org/support/article/creating-a-favicon/)

#### Q69. How would you write a text string containing "Hello World!" in a way that makes it possible for someone else to translate the string into a different language?

- [ ] `apply_filters( 'Hello World!', 'mytextdomain' );`
- [ ] `esc_html( 'Hello World!', 'mytextdomain' );`
- [ ] `$string = "Hello World!";`
- [x] `__( 'Hello World!', 'mytextdomain' );`

[Reference](https://wordpress.stackexchange.com/questions/231685/how-to-get-a-translated-string-from-a-language-other-than-the-current-one)

#### Q70. Which of these are best practices in accessibility?

- [ ] Do not skip heading levels.
- [ ] Be sure there is proper color contrast between background and text.
- [ ] If an activity can be completed with a mouse, it must also be accessible by keyboard.
- [x] all of these answers

#### Q71. JavaScript variables can hold many data types. Which data type does the following variable represent?

```js
var x = '16';
```

- [ ] Boolean
- [ ] Number
- [x] String
- [ ] Object

[Reference](https://www.w3schools.com/js/js_datatypes.asp)

#### Q72. You would use a post instead of a page when the content is **\_**.

- [ ] for a top-level menu item
- [ ] nested (has a parent/child relationship with another piece of content)
- [x] when the content is part of a blog.
- [ ] evergreen

#### Q73. The WordPress block editor contains a number of default blocks, including blocks for paragraphs, images, quotes, and shortcode. Blocks are grouped into categories to help users browse and discover them. Which is not a category provided by WordPress core?

- [ ] formatting
- [ ] widgets
- [ ] layout
- [x] shortcodes

#### Q74. What service is used to manage user profile photos across any WordPress site?

- [x] Gravatar
- [ ] WordPress.org
- [ ] None. Just upload a profile photo from your site user account.
- [ ] Profile Photo plugin

#### Q75. Which is not a benefit of DRY code?

- [ ] The code can be reused.
- [x] The code is less abstracted.
- [ ] The code is easier to read.
- [ ] The code is easier to maintain.

#### Q76. Which of these does not impact your site speed?

- [ ] caching
- [ ] your web host
- [x] inactive plugins
- [ ] content delivery network (CDN)

#### Q77. Where do you configure global settings for comments on your WordPress site?

- [ ] Tools screen
- [ ] wp-config.php
- [ ] cPanel
- [x] Discussion Settings

#### Q78. What can you not configure via wp-config.php?

- [x] changing the default user role
- [ ] changing the default wp_table prefix
- [ ] changing your site or WordPress address
- [ ] changing the default number of post revisions

#### Q79. When it comes to best practice for WordPress development, what is the preferred method for adding a custom post type (CPT) to a site?

- [ ] Add CPTs via phpMyAdmin.
- [x] Add CPTs via a plugin.
- [ ] Add CPTs via a parent theme.
- [ ] Add CPTs via a child theme.

[Reference](https://www.wpbeginner.com/wp-tutorials/how-to-create-custom-post-types-in-wordpress/)

#### Q80. What is a way you can both harden your site's security and improve how Google presents you site in search results?

- [x] Install an SSL certificate.
- [ ] Install a security plugin on your site.
- [ ] Use a third-party security monitoring service.
- [ ] Require user to log in to view content.

#### Q81. Review the HTML on line 1.The goal of the PHP on line 2 is to extract the field value and assign it to a variable prior to inserting into the database. What is wrong with this PHP code?

1. `<input type="text" id="title" name="title" />`
2. `$title = $_POST[ 'title' ]`

- [ ] The code sample does not allow for translation. It should use a translation function and look like this: `$title = __($_POST['title'])`
- [x] The code sample does not sanitize the form data. It should use the sanitize_text_field() function and look like this: `$title = sanitize_text_field($_POST['title']);`.
- [ ] There is no error. The code follows Wordpress best practice.
- [ ] The sample does not use GET method. It should be wrapped in the ger_post_field() function and look like this: `$title = get_post_field($_GET['title']);`.

#### Q82. Which of these is not a part of the internationalization and localization process?

- [ ] using a tool like Poedit to parse source code and extract translatable strings into a POT file.
- [x] translators translating the PO file, one for each language.
- [ ] installing/using the Wordpress Multilingual Plugin.
- [ ] using a gettext function to wrap transatable strings when writing code.

#### Q83. The REST API provides data, which is accessible to any client anonymously, as well as private data available only after authentication. How could you ensure that no one can anonymously access site data via the REST API?

- [ ] Disable the REST API via the site's wp-config.php file.
- [ ] Use the rest_authenticaton_errors() filter along with the is_user_logged_in() conditional to limit access to logged in users.
- [x] Use the Disable REST API plugin.
- [ ] Use the rest_authenticaton_errors() filter along with cookie authentication to limit access to logged in users.

#### Q84. Which of these refers to a WordPress security token that is used to verify that a request was made by the right person or client?

- [ ] Salt
- [ ] Cookie
- [x] Nonce
- [ ] Transient

[Reference](https://www.hostinger.com/tutorials/wordpress-nonce)
