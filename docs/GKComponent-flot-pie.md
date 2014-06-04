##gk-device-motion
`flot-pie` 可以協助使用者產生元餅圖，採用 flot-pie 的樣式。  

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
<td>class</td>
<td></td>
</tr>

<tr>
<td>style</td>
<td>直接編寫元件 DOM inline 樣式</td>
</tr>

<tr>
<td>width</td>
<td></td>
</tr>

<tr>
<td>height</td>
<td></td>
</tr>

<tr>
<td>radius</td>
<td></td>
</tr>

<tr>
<td>labelRadius</td>
<td></td>
</tr>

<tr>
<td>showLegend</td>
<td></td>
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
`flot-pie` 元件沒有提供 api。


<br/>
###Javascript 面板內容
元件拖拉進入設計區域後，會在 javascript 的編輯面板同步產生下列代碼：

	$(document).on("gkComponentsReady", function () {
	  var data = [{
	    label: 'Games',
	    data: 43
	  }, {
	    label: 'Social Networking',
	    data: 26
	  }, {
	    label: 'Entertainment',
	    data: 10
	  }, {
	    label: 'Utilities',
	    data: 10
	  }, {
	    label: 'News',
	    data: 2
	  }, {
	    label: 'Other',
	    data: 9
	  }];
	
	  $('#gk-64PH1x').gk('render', data);
	});


<br/>
----------
以上便是 `flot-pie` 的相關說明，如果想了解更多其他元件，請回 [元件清單列表](https://github.com/ezoapp/Learn-GK-Components)  

官方網站：[www.ezoui.com/app](http://www.ezoui.com/app)  
EZoApp 開發工具：[jqmdesigner.appspot.com/](http://jqmdesigner.appspot.com/)




