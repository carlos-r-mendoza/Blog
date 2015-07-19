---
layout: post
title:  "Android Studio: App With No Title Bar"
date:   2014-11-24 11:12:25
categories: android
---
Removing the title bar in Android Studio from an app is relatively simple.

1. You can preview different Android themes by clicking on the <strong>AppTheme button</strong> in Design view when looking at layouts.

<a href="https://carloscodes.files.wordpress.com/2014/11/appthemebutton1.png"><img class="wp-image-103 size-full" src="https://carloscodes.files.wordpress.com/2014/11/appthemebutton1.png" alt="Click on AppThemeButton" width="720" height="720" /></a> Click on AppThemeButton

2. Click on the <strong>AppTheme button</strong>, go to <strong>All</strong>, choose <strong>NoTitleBar</strong>, and click <strong>OK</strong>. This provides you with a preview of what you app will look like without a title bar.

[caption id="attachment_105" align="aligncenter" width="720"]<a href="https://carloscodes.files.wordpress.com/2014/11/select_theme_no_title_bar.jpg"><img class="wp-image-105 size-full" src="https://carloscodes.files.wordpress.com/2014/11/select_theme_no_title_bar.jpg" alt="Select 'No Title Bar' Theme" width="720" height="720" /></a> Select 'No Title Bar' Theme[/caption]

[caption id="attachment_110" align="alignnone" width="720"]<a href="https://carloscodes.files.wordpress.com/2014/11/app_preview_no_title_bar.png"><img class="size-full wp-image-110" src="https://carloscodes.files.wordpress.com/2014/11/app_preview_no_title_bar.png" alt="Preview of App With No Title Bar" width="720" height="720" /></a> Preview of App With No Title Bar[/caption]

3. You can also preview your app in devices using different screen sizes, including tablets, by clicking on the <strong>phone icon</strong> and choosing the <strong>Preview All Screen Sizes</strong> options in Design view when looking at layouts. To preview the look of your app in landscape or portrait orientation, click on the <strong>orientation icon</strong>.

[caption id="attachment_101" align="aligncenter" width="730"]<a href="https://carloscodes.files.wordpress.com/2014/11/preview_all_screen_sizes.png"><img class="wp-image-101 size-large" src="https://carloscodes.files.wordpress.com/2014/11/preview_all_screen_sizes.png?w=730" alt="Click on Phone Icon and Choose Preview All Screen Sizes" width="730" height="521" /></a> Click on Phone Icon and Choose Preview All Screen Sizes[/caption]

[caption id="attachment_100" align="aligncenter" width="720"]<a href="https://carloscodes.files.wordpress.com/2014/11/change_orientation.png"><img class="wp-image-100 size-full" src="https://carloscodes.files.wordpress.com/2014/11/change_orientation.png" alt="Preview Your App in Landscape or Portrait Orientation" width="720" height="720" /></a> Preview Your App in Landscape or Portrait Orientation[/caption]

4. Keep in mind that changing the theme using the <strong>AppTheme button only provides a preview</strong>. <strong>You must change the theme inside the styles.xml file</strong> to make the change permanent (<strong>res</strong> folder -&gt; <strong>values</strong> folder -&gt; <strong>styles.xml</strong> file).

5. In the <strong>styles.xml</strong> file, change the theme to one with no title bar (add a period to the end of the theme name and you should see a pop up with various theme options; choose the <strong>.NoActionBar</strong> theme).

[caption id="attachment_108" align="aligncenter" width="730"]<a href="https://carloscodes.files.wordpress.com/2014/11/change_sytlesxml_file.jpg"><img class="wp-image-108 size-large" src="https://carloscodes.files.wordpress.com/2014/11/change_sytlesxml_file.jpg?w=730" alt="Change Theme in the styles.xml file" width="730" height="535" /></a> Change Theme in the styles.xml file[/caption]

6. Go back to the Design view. Your app should no longer have a title bar!

7. Keep in mind that if you are using a newer version of Android Studio, that you should also change the theme in other styles.xml files that support newer versions of Android (e.g. when creating apps that support Google's new material design, you will notice that there is a folder titled <strong>values-v21</strong>; also change the theme in the<strong> styles.xml</strong> file found inside that folder).