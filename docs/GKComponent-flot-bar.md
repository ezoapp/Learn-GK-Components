##flot-bar
`flot-bar` 可以協助使用者產生 bar 的圖表，採用 flot-bar 的樣式。   

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
<td>xlabel</td>
<td></td>
</tr>

<tr>
<td>ylabel</td>
<td></td>
</tr>

<tr>
<td>mode</td>
<td></td>
</tr>

<tr>
<td>valueLabels</td>
<td></td>
</tr>

<tr>
<td>barWidth</td>
<td></td>
</tr>

<tr>
<td>xTicks</td>
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
`flot-bar` 元件沒有提供 api。


<br/>
###Javascript 面板內容
元件拖拉進入設計區域後，會在 javascript 的編輯面板同步產生下列代碼：

	$(document).on("gkComponentsReady", function () {
	  var data = [{
	    label: 'Games',
	    data: [
	      ['Games', 32]
	    ]
	  }, {
	    label: 'Facebook',
	    data: [
	      ['Facebook', 17]
	    ]
	  }, {
	    label: 'Browser',
	    data: [
	      ['Browser', 14]
	    ]
	  }, {
	    label: 'Social Messaging',
	    data: [
	      ['Social Messaging', 9.5]
	    ]
	  }, {
	    label: 'YouTube',
	    data: [
	      ['YouTube', 4]
	    ]
	  }, {
	    label: 'Entertainment',
	    data: [
	      ['Entertainment', 4]
	    ]
	  }, {
	    label: 'Utilities',
	    data: [
	      ['Utilities', 8]
	    ]
	  }, {
	    label: 'News',
	    data: [
	      ['News', 3]
	    ]
	  }, {
	    label: 'Other',
	    data: [
	      ['Other', 8.5]
	    ]
	  }];
	
	  $('#gk-64Aerd').gk('render', data);
	});

<br/>
----------
以上便是 `flot-bar` 的相關說明，如果想了解更多其他元件，請回 [元件清單列表](https://github.com/ezoapp/Learn-GK-Components)  

官方網站：[www.ezoui.com/app](http://www.ezoui.com/app)  
EZoApp 開發工具：[jqmdesigner.appspot.com/](http://jqmdesigner.appspot.com/)




