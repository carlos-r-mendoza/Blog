---
layout: post
title:  "Publishing an Android App on the Play Store"
date:   2014-11-15 11:12:25
categories: android
---
<a href="../img/publishing-an-android-app-on-the-play-store/play-store-publishing-console.png"><img class="size-large wp-image-85" src="../img/publishing-an-android-app-on-the-play-store/play-store-publishing-console.png" alt="Publishing an App on the Play Store" width="660" height="357" /></a> Publishing an App on the Play Store

I recently published my first Android App on Google's Play store, which you can find for free <a title="Amusing Facts Android App" href="https://play.google.com/store/apps/details?id=carlosrmendoza.com.amusingfacts" target="_blank">here</a>. Below I've listed the steps I took to publish the app. Keep in mind that these steps are for publishing a <strong>free app</strong> on the Play store. You can find out information on monetizing your app <a title="Monetize Android App Information Link" href="http://developer.android.com/distribute/monetize/index.html" target="_blank">here</a>.
<p style="text-align:center;"><strong>Steps to Publishing an Android App</strong></p>


<a href="../img/publishing-an-android-app-on-the-play-store/android-studio-runproguard-true.png"><img class="size-medium wp-image-87" src="../img/publishing-an-android-app-on-the-play-store/android-studio-runproguard-true.png" alt="Progard Tool" width="300" height="146" /></a> Make runProguard 'true'

<a href="../img/publishing-an-android-app-on-the-play-store/android-studio-proguard-rules-pro-file.png"><img class="wp-image-88 size-medium" src="../img/publishing-an-android-app-on-the-play-store/android-studio-proguard-rules-pro-file.png" alt="proguard-rules.pro file" width="300" height="114" /></a> proguard-rules.pro file
<ol>
	<li><strong>In Android Studio deactivate logging and disable the debugging option before you build your application for release</strong> (more information: <a title="Deactivate logging and disable debugging " href="http://developer.android.com/tools/publishing/preparing.html" target="_blank">http://developer.android.com/tools/publishing/preparing.html</a>)
<ul>
	<li>Use Proguard tool -&gt; go to build.gradle -&gt; make runProguard ‘true’ -&gt; rename getDefaultProguardFile to ‘proguard-android-optimize.txt’</li>
	<li>In the proguard-rules.pro file, copy and paste the following:-assumenosideeffects class android.util.Log {
public static boolean isLoggable(java.lang.String, int);
public static int v(...);
public static int i(...);
public static int w(...);
public static int d(...);
public static int e(...);
}</li>
</ul>
</li>
	<li><strong>Building a Release Ready APK</strong>
<ul>
	<li>In Android Studio, go to Build -&gt; Generate Signed APK -&gt; ‘Create new…’ Key store path (keep in mind that this will be the same to publish all subsequent apps under the same account, so make sure to store the key) -&gt; choose ‘release’ type apk</li>
	<li>This will create a release ready apk to upload to the Play store</li>
</ul>
</li>
	<li><strong>Google Play Developer Console </strong>(<a href="https://play.google.com/apps/publish">https://play.google.com/apps/publish</a>)
<ul>
	<li>Create account – it is $25 to create a publisher account (I believe this is a one time fee)</li>
	<li>Complete your account information</li>
	<li>Click on ‘+ Add new application’ button</li>
	<li>Click on ‘Upload APK to production’ button</li>
	<li>Complete the Store Listing (Icons)</li>
	<li>Click on the ‘Ready to Publish’ button</li>
	<li>Wait for about an hour, and your app should be on the Play store!</li>
</ul>
</li>
	<li><strong>Useful Resources</strong>
<ul>
	<li>Info for distributing app - <a title="Distributing App" href="http://developer.android.com/distribute/index.html" target="_blank">http://developer.android.com/distribute/index.html</a></li>
	<li>Launch Checklist - <a title="Launch Checklist" href="http://developer.android.com/distribute/tools/launch-checklist.html" target="_blank">http://developer.android.com/distribute/tools/launch-checklist.html</a></li>
	<li>Preparing App for Release - <a title="Preparing App for Release" href="http://developer.android.com/tools/publishing/preparing.html" target="_blank">http://developer.android.com/tools/publishing/preparing.html</a></li>
	<li>App Iconography - <a title="App Iconography" href="http://developer.android.com/design/style/iconography.html" target="_blank">http://developer.android.com/design/style/iconography.html</a></li>
</ul>
</li>
</ol>