---
layout: post
title:  "HTTP Status Codes"
date:   2015-04-17 11:12:25
categories: tool
---
HTTP is the protocol for transferring files across the World Wide Web, outlining how information is formatted and transmitted and the actions that browsers and web servers should take in response to certain actions.

Below are some of the most common Hypertext Transfer Protocol (HTTP) response status codes, which are responses provided by the web server and are often helpful when trying to identify the reason behind a problem.
<ul>
	<li><strong>200 OK</strong> - This is the standard response for a successful HTTP request.</li>
	<li><strong>201 Created</strong> - The request has executed, resulting in a new resource being created. This is often associated with POST requests.</li>
	<li><strong>301 Moved Permanently</strong> - The content requested has been moved and the current and any future requests should be directed to the URI provided.</li>
	<li><strong>400 Bad Request</strong> - The server is not able to or will not process the request due to an error perceived to be on the client side.</li>
	<li><strong>401 Unauthorized</strong> - Authentication is required and has failed or has yet to be provided.</li>
	<li><strong>403 Forbidden</strong> - The web server is configured to deny access to the resource requested by the client.</li>
	<li><strong>404 Not Found</strong> - The client successfully communicated with the web server but the resource requested was not found.</li>
	<li><strong>500 Internal Server Error</strong> - Generic error message when an unexpected condition is encountered and a more specific message is not suitable.</li>
	<li><strong>503 Service Unavailable </strong>- Currently the server is unavailable due to heavy traffic or down for maintenance. This is commonly a temporary state.</li>
</ul>