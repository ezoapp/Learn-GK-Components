##gk-device-motion
`gk-device-motion` 元件可以獲取手機或平板裝置的陀螺儀，進行三軸的運算判斷。  

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
Above is the description of `gk-device-motion`. For more information, please back to [GK-Components-List](https://github.com/ezoapp/Learn-GK-Components).

Offical Site：[www.ezoui.com/app/](http://www.ezoui.com/app/)  
EZoApp Designer：[jqmdesigner.appspot.com/](http://jqmdesigner.appspot.com/)




