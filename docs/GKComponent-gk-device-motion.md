##gk-device-motion
`gk-device-motion` 元件可以獲取手機或平板裝置的陀螺儀，進行三軸的運算判斷。  

<br/>
###元件位置
以下列出 `gk-device-motion` 元件可以放置的位置，以及哪些元件可以放入 `gk-device-motion` 裡頭。
<table>
<tr>
<th style="background:#ddd;">位置說明</th>
<th style="background:#ddd;">相關元件</th>
</tr>
<tr>
<td>gk-device-motion 可以放在哪些元件內？
</td>
<td>page</td>
</tr>
<tr>
<td>哪些元件可以放在 gk-device-motion 內？</td>
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
`gk-device-motion` 元件沒有提供 api。


<br/>
###Javascript 面板內容
元件拖拉進入設計區域後，會在 javascript 的編輯面板同步產生下列代碼：

	/*** code gen by gk-device-motion  ***/
	$(document).on("gkComponentsReady", function () {
	  function onSuccess(acceleration) {
	    var x = acceleration.x;
	    var y = acceleration.y;
	    var z = acceleration.z;
	    var times = acceleration.timestamp;
	    $("#gk-64HYJC").html("Acceleration X: " + x + "<br /> Acceleration Y: " + y + "<br /> Acceleration Z: " + z + "<br /> Timestamp: " + times + "<br />");
	  }
	
	  function onError(error) {
	    console.log("onError!");
	  }
	  if (navigator.accelerometer) {
	    var watchID = navigator.accelerometer.watchAcceleration(onSuccess, onError, {
	      frequency: 1000
	    });
	  }
	});


<br/>
----------
以上便是 `gk-device-motion` 的相關說明，如果想了解更多其他元件，請回 [元件清單列表](https://github.com/ezoapp/Learn-GK-Components)  

官方網站：[www.ezoui.com/app](http://www.ezoui.com/app)  
EZoApp 開發工具：[jqmdesigner.appspot.com/](http://jqmdesigner.appspot.com/)




