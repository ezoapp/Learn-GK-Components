## Learn GK Components ##
For more information, please visit [EZoApp Official Site](http://ezoui.com/) .  
![GK Components](https://raw.githubusercontent.com/ezoapp/Learn-GK-Components/master/img/banner.jpg)
  
## What is GK Components? ##
EZoApp's core values: reuse and modularization. User interfaces (UIs) that have been created can become modular components. You can create your own UI specifications and templates for application design to strengthen development standards.

## How to Use GK Components? ##

### Get the GK Object ###
GK is a jQuery plugin, and an implicit GK object is stored in the jQuery object. After GK finishes initialization, GK will fire `gkComponentsReady` event, then you are free to manipulate the GK object.

```javascript  
	// after gk finishes initialization, all gk components are ready to use...
	$(document).on("gkComponentsReady", function () {
	  // get the gk-obj
	  var gkObj = $(".selector").gk();
	  
	  // access the public attributes of the gk-obj
	  var foo = gkObj.foo;
	  
	  // call the public methods of the gk-obj and get the results returned
	  var result = gkObj.bar();
	});
```	

### Invoke API methods of the GK Object ###
After GK finishes initialization and fires `gkComponentsReady` event, and you can send arguments to invoke methods of the GK object. There are two equivalent ways to get the same result:

```javascript 
	// always waiting gk finishes initialization...
	$(document).on("gkComponentsReady", function () {
	  // get the gk-obj and send arguments to a method
	  $(".selector").gk().method(args..);
	  
	  // this syntax is fine also
	  $(".selector").gk("method", args...);
	}); 
```

## Components list ##
This is a list of all the GK Components. Click on the links and know how to use the gk-components.

### JQM Components ###
* [header](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-header.md)
* [footer](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-footer.md)
* [grid](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-grid.md)
* [tabbar](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-tabbar.md)
* [navbar](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-navbar.md)
	* [navBtn](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-navbtn.md)
* [gk-text](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-gk-text.md)
* [text-input](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-text-input.md) 
* [range-input](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-range-input.md)
* [search-input](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-search-input.md)
* [date-input](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-date-input.md)
* [collapsible-set](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-collapsible-set.md)
	* [collapsible](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-collapsible.md) ( api )
* [icon](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-icon.md)
* [button](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-button.md) 
* [listview](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-listview.md)
	* [listview-li](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-listview-li.md)
	* [list-divider](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-list-divider.md)
* [controlgroup-radio](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-controlgroup-radio.md)
	* [radio-button](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-radio-button.md)
* [controlgroup-checkbox](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-controlgroup-checkbox.md)
	* [checkbox-button](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-checkbox-button.md)
* [flipswitch](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-flipwitch.md)
* [selectmenu](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-selectmenu.md) ( api )
* [textarea-input](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-textarea-input.md) ( api )
* [jqm-table](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-jqm-table.md)

### Extension Components ###
* [youtube](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-youtube.md)
* [image](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-image.md)
* [mobipick](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-mobipick.md) ( property, api )
* [gmap](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-gmap.md) ( property, api )
* [raty](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-raty.md) ( property, api )
* [bxslider](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-bxslider.md) ( property, api )
* [qrcode](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-qrcode.md) ( property, api )
* [imggallery](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-imggallery.md) ( property, api )
* [json-listview](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-json-listview.md)
* [page-listview](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-page-listview.md)
* [capture-photo](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-capture-photo.md)
* [gk-position](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-gk-position.md)
* [gk-device-motion](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-gk-device-motion.md)
* [flot-pie](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-flot-pie.md)
* [flot-bar](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-flot-bar.md) ( property, api )
* [flot-stacking](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-flot-stacking.md) ( property, api )
* [flot-line](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-flot-line.md) ( property, api )
* [linechart](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-linechart.md) ( api )
* [rss-news](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-rss-news.md) ( api )
* [barcode-scanner](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-barcode-scanner.md) 
* [json-selectmenu](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-json-selectmenu.md) 

## Contact ##
If you have any questions about the components, or want to join us, please contact us.  

* EZoApp Official Site: [ezoui.com](http://ezoui.com/)
* Phone: +886-7-535-0101 # 35505
* E-mail: [EZoService@icsc.com.tw](mailto:service@ezoui.com)  
* Facebook: [www.facebook.com/EZoUI](http://www.facebook.com/EZoUI)  
* Google+: [plus.google.com/117990746163074166131](http://plus.google.com/117990746163074166131)  
* blog: [EZoUI.wordpress.com](http://EZoUI.wordpress.com)

