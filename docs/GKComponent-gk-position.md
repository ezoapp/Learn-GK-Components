##gk-position
`gk-position` 元件可以獲取手機或平板裝置 GPS 座標。 

<br/>
###元件位置
以下列出 `gk-position` 元件可以放置的位置，以及哪些元件可以放入 `gk-position` 裡頭。
<table>
<tr>
<th style="background:#ddd;">位置說明</th>
<th style="background:#ddd;">相關元件</th>
</tr>
<tr>
<td>gk-position 可以放在哪些元件內？
</td>
<td>page</td>
</tr>
<tr>
<td>哪些元件可以放在 gk-position 內？</td>
<td>無</td>
</tr>
</table>

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
以上便是 `gk-position` 的相關說明，如果想了解更多其他元件，請回 [元件清單列表](https://github.com/ezoapp/Learn-GK-Components)  

官方網站：[www.ezoui.com/app](http://www.ezoui.com/app)  
EZoApp 開發工具：[jqmdesigner.appspot.com/](http://jqmdesigner.appspot.com/)




