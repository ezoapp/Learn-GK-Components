##Glinechart
`linechart` 元件會由使用者在 javascript 中的陣列，產生對應的線狀圖表。

<br/>
###元件位置

以下列出 `linechart` 元件可以放置的位置，以及哪些元件可以放入 `linechart` 裡頭。
<table>
<tr>
<th style="background:#ddd;">位置說明</th>
<th style="background:#ddd;">相關元件</th>
</tr>
<tr>
<td>linechart 可以放在哪些元件內？
</td>
<td>
<ul>
<li>page</li>
<li>header</li>
<li>collapsible</li>
<li>controlgroup</li>
</ul>
</td>
</tr>
<tr>
<td>哪些元件可以放在 linechart 內？</td>
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

</table>

<br/>
###API
`linechart` 元件沒有提供 api。

<br/>
###Javascript 面板內容
元件拖拉進入設計區域後，會在 javascript 的編輯面板同步產生下列代碼：

	;
	$(document).one("pageshow", "#home", function aa() {
	  var chart = $("#gk-64qWff").gk("render", [0, 1, 2, 3, 4, 5], [
	    [1, 3, 5, 7, 9, 7],
	    [2, 5, 3, 1, 9, 12]
	  ], {
	    "colors": ["#f00", "#0000FF"],
	    nostroke: false,
	    "axis": "0 0 1 1",
	    "symbol": "circle",
	    smooth: true
	  });
	  chart.paper.label(25, 150, "Score").attr({
	    fill: "#fff",
	    stroke: "#000",
	    "stroke-width": 1
	  });
	}); 

<br/>
----------
以上便是 `linechart` 的相關說明，如果想了解更多其他元件，請回 [元件清單列表](https://github.com/ezoapp/Learn-GK-Components)  

官方網站：[www.ezoui.com/app](http://www.ezoui.com/app)  
EZoApp 開發工具：[jqmdesigner.appspot.com/](http://jqmdesigner.appspot.com/)




