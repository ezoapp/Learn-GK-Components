#barcode-scanner
`barcode-scanner` allows the user to scan the barcode. It renders a button widget which will trigger the barcode scanner when it is clicked.

## Sample App
![Sample App](https://raw.githubusercontent.com/ezoapp/Learn-GK-Components/master/img/barcode-scanner/app.png)

![Barcode Scanner](https://raw.githubusercontent.com/ezoapp/Learn-GK-Components/master/img/barcode-scanner/scan.png)

### sample code
HTML
```html
<div id="home" data-role="page">
  <div data-role="header" data-position="fixed">
    <h3>Barcode Scanner</h3>
  </div>
  <div role="main" class="ui-content">
    <div class="ui-field-contain">
      <label for="code">code</label>
      <input type="text" name id="code">
    </div>
    <a id="gk-429TpIW-btn" class="ui-btn" is="barcode-scanner">scan barcode</a>
  </div>
</div>
```
Javascript
```javascript  
	$(document).on("gkComponentsReady", function () {
	  $("#gk-429TpIW-btn").click(function () {
	    cordova.plugins.barcodeScanner.scan(function (result) {
	    	// read the result of scanning
	      $('#code').val(result.text);
	    }, function (error) {
	      alert("Scanning failed: " + error);
	    });
	  });
	}); 
```	
 
### Properties
property			| setting
---						| ---
N.A.						| N.A. 

 
### Content
The label of the button.
 
### API
Please refer the [official site](https://github.com/wildabeast/BarcodeScanner) of the `BarcodeScanner` plugin.
 

----------
Above is the description of `barcode-scanner`. For more information, please back to [GK-Components-List](https://github.com/ezoapp/Learn-GK-Components).

EZoApp Official Site: [ezoui.com](http://ezoui.com/)



