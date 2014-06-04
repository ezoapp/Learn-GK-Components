##flot-stacking
`flot-stacking` 可以協助使用者產生 stacking 的圖表，採用 flot-stacking 的樣式。 

<br/>
###元件位置
以下列出 `flot-stacking` 元件可以放置的位置，以及哪些元件可以放入 `flot-stacking` 裡頭。
<table>
<tr>
<th style="background:#ddd;">位置說明</th>
<th style="background:#ddd;">相關元件</th>
</tr>
<tr>
<td>flot-stacking 可以放在哪些元件內？
</td>
<td>
<ul>
<li>page</li>
<li>content</li>
<li>collapsible</li>
<li>controlgroup</li>
</ul>
</td>
</tr>
<tr>
<td>哪些元件可以放在 flot-stacking 內？</td>
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
`flot-stacking` 元件沒有提供 api。


<br/>
###Javascript 面板內容
元件拖拉進入設計區域後，會在 javascript 的編輯面板同步產生下列代碼：

	  $(document).on("gkComponentsReady", function () {
	    var data = [{
	      label: 'Apps',
	      data: [
	        [0, 80],
	        [1, 86],
	      ],
	      color: '#50b4f6'
	    }, {
	      label: 'Mobile Web',
	      data: [
	        [0, 20],
	        [1, 14],
	      ],
	      color: '#9e9e9e'
	    }];
	
	    var options = {
	      yaxis: {
	        autoscaleMargin: 0.2,
	      }
	    };
	
	    $('#gk-64Kx9B').gk('render', data, options);
	  });

<br/>
----------
以上便是 `flot-stacking` 的相關說明，如果想了解更多其他元件，請回 [元件清單列表](https://github.com/ezoapp/Learn-GK-Components)  

官方網站：[www.ezoui.com/app](http://www.ezoui.com/app)  
EZoApp 開發工具：[jqmdesigner.appspot.com/](http://jqmdesigner.appspot.com/)




