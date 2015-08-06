---
layout: post
title:  "Android Studio: App With No Title Bar"
date:   2014-11-24 11:12:25
categories: android development
author: Carlos R. Mendoza
<!-- permalink: -->
---
Removing the title bar in Android Studio from an app is relatively simple.

1. You can preview different Android themes by clicking on the <strong>AppTheme button</strong> in Design view when looking at layouts.

<a href="../img/android-studio-app-with-no-title-bar/apptheme-button.png"><img class="wp-image-103 size-full" src="../img/android-studio-app-with-no-title-bar/apptheme-button.png" alt="Click on AppThemeButton" width="720" height="720" /></a> Click on AppThemeButton

2. Click on the <strong>AppTheme button</strong>, go to <strong>All</strong>, choose <strong>NoTitleBar</strong>, and click <strong>OK</strong>. This provides you with a preview of what you app will look like without a title bar.

<a href="../img/android-studio-app-with-no-title-bar/select-theme-no-title-bar.jpg"><img class="wp-image-105 size-full" src="../img/android-studio-app-with-no-title-bar/select-theme-no-title-bar.jpg" alt="Select 'No Title Bar' Theme" width="720" height="720" /></a> Select 'No Title Bar' Theme

<a href="../img/android-studio-app-with-no-title-bar/preview-no-title-bar.png"><img class="size-full wp-image-110" src="../img/android-studio-app-with-no-title-bar/preview-no-title-bar.png" alt="Preview of App With No Title Bar" width="720" height="720" /></a> Preview of App With No Title Bar

3. You can also preview your app in devices using different screen sizes, including tablets, by clicking on the <strong>phone icon</strong> and choosing the <strong>Preview All Screen Sizes</strong> options in Design view when looking at layouts. To preview the look of your app in landscape or portrait orientation, click on the <strong>orientation icon</strong>.

<a href="../img/android-studio-app-with-no-title-bar/preview-all-screen-sizes.png"><img class="wp-image-101 size-large" src="../img/android-studio-app-with-no-title-bar/preview-all-screen-sizes.png" alt="Click on Phone Icon and Choose Preview All Screen Sizes" width="730" height="521" /></a> Click on Phone Icon and Choose Preview All Screen Sizes

<a href="../img/android-studio-app-with-no-title-bar/preview-change-orientation.png"><img class="wp-image-100 size-full" src="../img/android-studio-app-with-no-title-bar/preview-change-orientation.png" alt="Preview Your App in Landscape or Portrait Orientation" width="720" height="720" /></a> Preview Your App in Landscape or Portrait Orientation

4. Keep in mind that changing the theme using the <strong>AppTheme button only provides a preview</strong>. <strong>You must change the theme inside the styles.xml file</strong> to make the change permanent (<strong>res</strong> folder -&gt; <strong>values</strong> folder -&gt; <strong>styles.xml</strong> file).

5. In the <strong>styles.xml</strong> file, change the theme to one with no title bar (add a period to the end of the theme name and you should see a pop up with various theme options; choose the <strong>.NoActionBar</strong> theme).

<a href="../img/android-studio-app-with-no-title-bar/change-theme-sytlesxml-file.jpg"><img class="wp-image-108 size-large" src="../img/android-studio-app-with-no-title-bar/change-theme-sytlesxml-file.jpg" alt="Change Theme in the styles.xml file" width="730" height="535" /></a> Change Theme in the styles.xml file

6. Go back to the Design view. Your app should no longer have a title bar!

7. Keep in mind that if you are using a newer version of Android Studio, that you should also change the theme in other styles.xml files that support newer versions of Android (e.g. when creating apps that support Google's new material design, you will notice that there is a folder titled <strong>values-v21</strong>; also change the theme in the<strong> styles.xml</strong> file found inside that folder).