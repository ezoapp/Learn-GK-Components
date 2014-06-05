##capture-photo
`capture-photo` 元件可以使用手機或平板的相機裝置進行拍照的功能  

<br/>
###Properties
<table>

<tr>
<th style="background:#ddd;">property</th>
<th style="background:#ddd;">setting</th>
</tr>

<tr>
<td>id</td>
<td>元件的 id</td>
</tr>

<tr>
<td>style</td>
<td>直接編寫元件 DOM inline 樣式</td>
</tr>

<tr>
<td>isUseGKComponent</td>
<td><ul>
<li>true：轉換為 GK 元件 ( 可使用 GK 元件 API )a</li>
<li>false：不轉換為 GK 元件</li>
</ul></td>
</tr>

</table>

<br/>
###API
`capture-photo` 元件沒有提供 api。


<br/>
###Javascript 面板內容
元件拖拉進入設計區域後，會在 javascript 的編輯面板同步產生下列代碼：

	/*** code gen by capture-photo  ***/
	$(document).on("gkComponentsReady", function () {
	  $("#gk-64jIRT-btn").on("click", function () {
	    if (navigator.camera) {
	      navigator.camera.getPicture(
	        // Called when a photo is successfully retrieved
	        function (imgURI) {
	          // Set image
	          $("#gk-64jIRT-img").attr("src", imgURI);
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




