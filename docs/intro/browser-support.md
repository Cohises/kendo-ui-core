---
title: Supported Browsers
page_title: Supported browsers
previous_url: /technical-requirements.html, /getting-started/technical-requirements, /browsers-support
description: "Supported browsers, platform support and prerequisites for best performance when working with Kendo UI."
position: 6
---

# Supported Browsers

Kendo UI components are designed to support all major browsers and to operate without the worries of cross-browser compatibility, standards compliance or touch-device support. 

In this section:  

* [Supported Desktop Browsers](#supported-desktop-browsers)  
* [Supported Operating Systems](#supported-operating-systems)
* [Other Prerequisites](#other-prerequisites)

## Supported Desktop Browsers

### Kendo UI Core and Web Widgets

| Browser			| Supported Versions			|
| :---------------- | :---------------------------- | 
| Internet Explorer | 7 or later					|
| Chrome          	| 21 or later					|
| Firefox          	| [Current and ESR releases](https://en.wikipedia.org/wiki/History_of_Firefox#Release_history) ([What is ESR?](https://www.mozilla.org/en-US/firefox/organizations/faq/))|
| Opera	        	| 15 or later					|
| OS X Safari    	| [6.2.6 or later](https://en.wikipedia.org/wiki/Safari_version_history#Mac)|

[List of Kendo UI Components](http://docs.telerik.com/kendo-ui/intro/list-of-widgets)

### Kendo UI Mobile Widgets

| Browser			| Supported Versions			|
| :---------------- | :---------------------------- | 
| Internet Explorer | 10 or later					|
| Chrome          	| 21 or later					|
| Firefox          	| Not supported					|
| Opera	        	| 15 or later					|
| OS X Safari    	| [6.2.6 or later](https://en.wikipedia.org/wiki/Safari_version_history#Mac)|

[List of Kendo UI Components](http://docs.telerik.com/kendo-ui/intro/list-of-widgets)

### Kendo UI DataViz Widgets

##### Fully Supported Desktop Browsers 

| Browser			| Supported Versions			|
| :---------------- | :---------------------------- | 
| Internet Explorer | 9 or later					|
| Chrome          	| 21 or later					|
| Firefox          	| [Current and ESR releases](https://en.wikipedia.org/wiki/History_of_Firefox#Release_history) ([What is ESR?](https://www.mozilla.org/en-US/firefox/organizations/faq/))|
| Opera	        	| 15 or later					|
| OS X Safari    	| [6.2.6 or later](https://en.wikipedia.org/wiki/Safari_version_history#Mac)|
| iOS Safari		| iOS 8 or later				|
| Chrome for Mobile | 21 or later					|

##### Desktop Browsers with Limited Support

Internet Explorer 6, 7 and 8 are supported with the following limitations:  

* PDF and image export is not supported
* Text rotation is not supported by the 64-bit versions
* Gradients in pie and donut charts are not supported  

Internet Explorer 10 is supported with the following limitations:  
  
* Dashed lines in canvas are not supported, which affects the image export as well
* Android 2.x, therefore, uses non-interactive canvas output

[List of Kendo UI Components](http://docs.telerik.com/kendo-ui/intro/list-of-widgets)

### Important Notes

* Since Internet Explorer 11 was released in October 2013, look up the Q3 2013 SP2 (2013.3.1324) or a more recent Kendo UI version if you need support for it
* Browsers in beta stage are not supported
* [Quirks mode](http://www.quirksmode.org/css/quirksmode.html) is not supported. Always specify a [DOCTYPE](http://reference.sitepoint.com/html/doctypes). Recommended DOCTYPES include `HTML5`, `XHTML 1.1`, `XHTML 1.0 Strict` and `HTML4 Strict`. The `HTML4 Transitional` DOCTYPE fires the Quirks mode and should not be used. `XHTML 1.0 Transitional` works well in most cases, but may cause issues with the vertical positioning of icons. The correct syntax for [all DOCTYPES](http://www.w3.org/QA/2002/04/valid-dtd-list.html) is provided on the [W3C website](http://www.w3.org/).
* Internet Explorer compatibility modes are not supported. These modes can exhibit different behavior and rendering bugs as compared to the browser versions they emulate. 
* It is highly recommendable to use [Internet Explorer Edge mode](http://blogs.msdn.com/b/ie/archive/2010/06/16/ie-s-compatibility-features-for-site-developers.aspx) via a META tag or an HTTP header

       <meta http-equiv="X-UA-Compatible" content="IE=edge" />

* Kendo UI uses a progressive enhancement for its CSS styling. As a result, old and obsolete browsers may ignore CSS3 styles, such as rounded corners and linear gradients.

### Internet Explorer As an Embedded Browser in a Desktop Application

Internet Explorer behaves differently when embedded inside a desktop (WinForms) application. It reports to support pointer events, but actually doesn't. As a result, some events, on which Kendo UI relies, are not fired. In order to avoid this problem, the following JavaScript code must be executed before the Kendo UI scripts are registered:

```
<script>
    window.MSPointerEvent = null;
    window.PointerEvent = null;
</script>
```

## Supported Operating Systems

| Platform			| Version				|
| :---------------- | :-------------------- | 
| Windows			| XP or later			|
| Windows Server  	| Server 2003 or later	|
| OS X          	| 10.5 or later			|
| Android        	| 2.3 or later			|
| iOS		    	| 6.0 or later			|
| BlackBerry        | 10.0 or later			|
| Windows Phone    	| 8.0 or later			|
| Chrome for Mobile	| Any version			|

### Important Notes

* Kendo UI DataViz widgets support only the Canvas rendering mode in Android 2.3
* Hybrid mouse and touch-screen devices are supported; for example, Internet Explorer 10, Chrome and Firefox on Windows 8
 
## Other Prerequisites

* Enable JavaScript on all browsers

Tips and tricks:  

* Check **Disable Script Debugging** from your browser configuration options
* Activate Caching in Internet Explorer