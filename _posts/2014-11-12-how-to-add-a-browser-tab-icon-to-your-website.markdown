---
layout: post
title:  "How to Add a Browser Tab Icon to Your Website"
date:   2014-11-12 11:12:25
categories: web
---
[caption id="attachment_40" align="aligncenter" width="300"]<a href="https://carloscodes.files.wordpress.com/2014/11/browser_tab_icon.png"><img class="size-medium wp-image-40" src="https://carloscodes.files.wordpress.com/2014/11/browser_tab_icon.png?w=300" alt="Browser Tab Icon Example" width="300" height="36" /></a> Browser Tab Icon Example[/caption]

The little tab browser icons that you have probably noticed while surfing the web are known as <a title="favicons" href="http://en.wikipedia.org/wiki/Favicon" target="_blank">favicons</a> and not only appear on the browser tab, but also next to a site's name on bookmark lists and desktop shortcuts.

How do you add a tab browser icon to your html page?

Keep in mind that a favicon needs to be <strong>16x16 pixels</strong> in size and a <strong>.ico file</strong>. Luckily, there are online tools that allow you to resize and convert your image to a .ico file all at once! For my <a title="Portfolio Site" href="http://carlosrmendoza.com" target="_blank">portfolio site</a>, I used <a title="convert image file to .ico format" href="http://image.online-convert.com/convert-to-ico" target="_blank">online-convert.com</a> to convert my .png image file to a 16X16 pixels .ico file.

<strong>Steps to Add a Browser Tab Icon to Your HTML Page</strong>
<ol>
	<li>Create the icon that you wish to display on the tab browser.
<ul>
	<li>Do not worry too much about image size and go ahead and save the file as a .png or .jpg file. You can later use an online converter to resize and to change the file format of your image.</li>
</ul>
</li>
	<li>Go to <a title="convert image file to .ico format" href="http://image.online-convert.com/convert-to-ico" target="_blank">online-convert.com</a>, convert your image to a .ico file, and resize your image to 16X16 pixels.

[caption id="attachment_48" align="aligncenter" width="660"]<a href="http://image.online-convert.com/convert-to-ico"><img class="wp-image-48 size-large" src="https://carloscodes.files.wordpress.com/2014/11/online-convert-com.png?w=660" alt="Resizing your image and saving it as a .ico file." width="660" height="434" /></a> Resizing your image and saving it as a .ico file.[/caption]</li>
	<li>Save your icon image inside the img file in your website's directory.</li>
	<li>Within the &lt;head&gt; tag of your html file insert the following &lt;link&gt; tag:
<ul>
	<li>&lt;link rel="shortcut icon" href="img/nameofyouriconfile.ico"&gt;</li>
	<li>Keep in mind that href should point exactly to where your image is located within your website's directory in relation to the html document.</li>
</ul>
</li>
	<li>Save everything, make sure to upload files to your host if your site is live, and refresh the browser. You should now have a tab browser icon displaying for your html file!</li>
</ol>