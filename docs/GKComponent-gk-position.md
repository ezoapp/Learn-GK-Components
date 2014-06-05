##gk-position
`gk-position` 元件可以獲取手機或平板裝置 GPS 座標。 

<br/>
###屬性設定
<table>

<tr>
<th style="background:#ddd;">屬性</th>
<th style="background:#ddd;">設定</th>
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
`gk-position` 元件沒有提供 api。


<br/>
###Javascript 面板內容
元件拖拉進入設計區域後，會在 javascript 的編輯面板同步產生下列代碼：

	/*** code gen by gk-position  ***/
	;
	$(document).on("gkComponentsReady", function () {
	  function onSuccess(position) {
	    var latitude = position.coords.latitude;
	    var longitude = position.coords.longitude;
	    $("#gk-64I0QA").html("Latitude: " + latitude + "<br /> Longitude: " + longitude);
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


<br/>
----------
Above is the description of `gk-position`. For more information, please back to [GK-Components-List](https://github.com/ezoapp/Learn-GK-Components).

Offical Site：[www.ezoui.com/app/](http://www.ezoui.com/app/)  
EZoApp Designer：[jqmdesigner.appspot.com/](http://jqmdesigner.appspot.com/)




