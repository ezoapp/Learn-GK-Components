# gmap
`gmap` allows the user to set the way through to complete Google Map display.


### Properties
property			| setting
---						| ---
id						| component's id
style					| style attribute of the html element 
class					| class attribute of the html element
key						| key of Google Map api, about usage limits please check [developers' guide](https://developers.google.com/maps/documentation/javascript/usage) 
sensor				| true or false, use device's sensor (e.g. gps) or not
address				| ***deprecated.***<br/> the address of the map, recommended using the tag content (representing **location**) instead  
mapTypeId			| rendering type of Google Map, `roadmap` type defaulted
markerTitle		| default title tip of map marker
markerIcon		| default icon image url of map marker
markerVisible | true or false, default map marker shown or not

### Content
The **location** setting of the Google Map. This value accepts both **`"latitude, longitude"`** data format for precise position and free-style string for address input.

### API
- **location**:
	- **`$(".selector").gk().location()`**
	
	> Get the current value of the location setting. <br/>
	
	- **`$(".selector").gk().location( value )`**
	
	> Set the location that the center of the map will be posited. <br/>
	> **value** <br/>
	> Type: String <br/>
	> Accepts both **`"latitude, longitude"`** data format for precise position and free-style string for address input. <br/>


- **address**:
	- **`$(".selector").gk().address( value )`**
	
	> ***deprecated.*** <br/> 
	> Posit the center of the map by the given address. Encourage using the **`location`** function instead.<br/>
	> **value** <br/>
	> Type: String <br/>
	> A string representing to a place. <br/>	


- **geocode**:
	- **`$(".selector").gk().onclick( address, function(result) )`**
	
	> Convert an address to **lat-lng** result and attach a function to handle the data. <br/>
	> **address** <br/>
	> Type: String <br/>
	> A place desired to get the **lat-lng** result. <br/>	
	> **function(result)** <br/>
	> Type: Function() <br/>
	> A callback function to receive the result returned by Google Map Geocoder while the geocode request succeeds. <br/>


- **nowPos**:
	- **`$(".selector").gk().addMarker( title, icon, visible )`**
	
	> Add a map marker according to the current position. <br/>
	> **title** <br/>
	> Type: String or undefined <br/>
	> The title tip of the map marker. Use default `markerTitle` while given undefined. <br/>
	> **icon** <br/>
	> Type: String or undefined <br/>
	> The icon image url of the map marker. Use default `markerIcon` while given undefined. <br/>	
	> **visible** <br/>
	> Type: Boolean or undefined <br/>
	> The location that the map marker was added by. Use default `markerVisible` while given undefined. <br/>


- **addMarker**:
	- **`$(".selector").gk().addMarker( location, title, icon, visible )`**
	
	> Add a map marker according to the given location.<br/>
	> **location** <br/>
	> Type: String <br/>
	> The location that the map marker will be added by. <br/>
	> **title** <br/>
	> Type: String or undefined <br/>
	> The title tip of the map marker. Use default `markerTitle` while given undefined. <br/>
	> **icon** <br/>
	> Type: String or undefined <br/>
	> The icon image url of the map marker. Use default `markerIcon` while given undefined. <br/>	
	> **visible** <br/>
	> Type: Boolean or undefined <br/>
	> The location that the map marker was added by. Use default `markerVisible` while given undefined. <br/>


- **removeMarker**:
	- **`$(".selector").gk().markerIcon( value )`**
	
	> Remove the map marker of the given location if exists. <br/>
	> **value** <br/>
	> Type: String <br/>
	> The location that the map marker was added by. <br/>


- **markerTitle**：  
	- **`$(".selector").gk().markerTitle()`**
	
	> Get the current title setting of the default map marker. <br/>
	
	- **`$(".selector").gk().markerTitle( value )`**
	
	> Set the title property of the default map marker. <br/>
	> **value** <br/>
	> Type: String <br/>
	> A string indicating the title tip of the default map marker. <br/>
	

- **markerIcon**:
	- **`$(".selector").gk().markerIcon()`**
	
	> Get the current icon setting of the default map marker. <br/>
	
	- **`$(".selector").gk().markerIcon( value )`**
	
	> Set the icon property of the default map marker. <br/>
	> **value** <br/>
	> Type: String <br/>
	> A string indicating the icon image url of the default map marker. <br/>


- **markerVisible**:
	- **`$(".selector").gk().markerVisible()`**
	
	> Get the current visible setting of the default map marker. <br/>
	
	- **`$(".selector").gk().markerVisible( value )`**
	
	> Set the visible property of the default map marker. <br/>
	> **value** <br/>
	> Type: Boolean <br/>
	> A Boolean indicating whether the default map marker should be shown. <br/>


- **onclick**:
	- **`$(".selector").gk().onclick( function(data) )`**
	
	> Attach a click event handler function for the Google Map event listener. <br/>
	> **function(data)** <br/>
	> Type: Function() <br/>
	> A callback function to receive the `lat-lng` data returned by Google Map while the click event is triggered. <br/>


- **height**:
	- **`$(".selector").gk().height()`**

	> Get the current height value of the element. <br/>
	
	- **`$(".selector").gk().height( value )`**
	
	> Set the height property of the element and resize the map. <br/>
	> **value** <br/>
	> Type: String or Number <br/>
	> An integer representing the number of pixels, or an integer along with an optional unit. <br/>


- **width**:  
	- **`$(".selector").gk().width()`**
	
	> Get the current width value of the element. <br/>
	
	- **`$(".selector").gk().width( value )`**
	
	> Set the width property of the element and resize the map.<br/>
	> **value** <br/>
	> Type: String or Number <br/>
	> An integer representing the number of pixels, or an integer along with an optional unit. <br/>


- **zoom**:  
	- **`$(".selector").gk().zoom()`**
	
	> Get the current zoom value of the map. <br/>
	
	- **`$(".selector").gk().zoom( value )`**
	
	> Set the zoom property of the map and rescale the map. <br/>
	> **value** <br/>
	> Type: String or Number <br/>
	> An integer number representing the scale of map zoom. <br/>


- **map**:  
	- **`$(".selector").gk().map()`**
	
	> Get the google map object. <br/>
	
	- **`$(".selector").gk().map( googleMap )`**
	
	> Replace the google map object. <br/>
	> **googleMap** <br/>
	> Type: Object <br/>
	> An instance of google.maps.Map . <br/>

----------
Above is the description of `gmap`. For more information, please back to [GK-Components-List](https://github.com/ezoapp/Learn-GK-Components).

EZoApp Official Site: [ezoui.com](http://ezoui.com/)



