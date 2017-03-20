## gk-position
`gk-position` can get GPS coordinates of the phone or tablet device.

### Properties
<table>

<tr>
<th style="background:#ddd;">property</th>
<th style="background:#ddd;">setting</th>
</tr>

<tr>
<td>id</td>
<td>Component's id</td>
</tr>

<tr>
<td>style</td>
<td>HTML inline style</td>
</tr>

</table>

### API
None


### Javascript Code
After dragging the component into the design panel, in javascript editor panel, and it will generate the code ( `#componentId` is the component's id )：

	/*** code gen by gk-position  ***/
	;
	$(document).on("gkComponentsReady", function () {
	  function onSuccess(position) {
	    var latitude = position.coords.latitude;
	    var longitude = position.coords.longitude;
	    $("#componentId").html("Latitude: " + latitude + "<br /> Longitude: " + longitude);
	  }
	
	  function onError(error) {
	    // onError Callback receives a PositionError object  
	  }
	  if (navigator.geolocation) {
	    var watchID = navigator.geolocation.watchPosition(onSuccess, onError, {
	      timeout: 10000
	    });
	  }
	});


----------
Above is the description of `gk-position`. For more information, please back to [GK-Components-List](https://github.com/ezoapp/Learn-GK-Components).

EZoApp Official Site: [ezoui.com](http://ezoui.com/)




