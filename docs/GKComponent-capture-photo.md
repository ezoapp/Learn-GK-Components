##capture-photo
`capture-photo` can use a camera phone or tablet device to take pictures.

<br/>
###Properties
<table>

<tr>
<th style="background:#ddd;">property</th>
<th style="background:#ddd;">setting</th>
</tr>

<tr>
<td>id</td>
<td>Component's id</td>
</tr>

</table>

<br/>
###API
None


<br/>
###Javascript Code
After dragging the component into the design panel, in javascript editor panel, and it will generate the code ( `#componentId` is the component's id )：

	/*** code gen by capture-photo  ***/
	$(document).on("gkComponentsReady", function () {
	  $("#componentId").on("click", function () {
	    if (navigator.camera) {
	      navigator.camera.getPicture(
	        // Called when a photo is successfully retrieved
	        function (imgURI) {
	          // Set image
	          $("#componentId").attr("src", imgURI);
	        },
	        // Called if something bad happens
	        function (msg) {
	          alert("Failed because: " + msg);
	        },
	        // Camera options
	        {
	          quality: 100,
	          destinationType: navigator.camera.DestinationType.FILE_URI,
	          sourceType: Camera.PictureSourceType.CAMERA,
	          encodingType: Camera.EncodingType.JPEG,
	          saveToPhotoAlbum: true
	        });
	    }
	  });
	});


<br/>
----------
Above is the description of `capture-photo`. For more information, please back to [GK-Components-List](https://github.com/ezoapp/Learn-GK-Components).

Offical Site：[www.ezoui.com/app/](http://www.ezoui.com/app/)  
EZoApp Designer：[jqmdesigner.appspot.com/](http://jqmdesigner.appspot.com/)




