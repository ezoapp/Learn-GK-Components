##Glinechart
`linechart` 元件會由使用者在 javascript 中的陣列，產生對應的線狀圖表。

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

</table>

<br/>
###API
None

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
Above is the description of `linechart`. For more information, please back to [GK-Components-List](https://github.com/ezoapp/Learn-GK-Components).

Offical Site：[www.ezoui.com/app/](http://www.ezoui.com/app/)  
EZoApp Designer：[jqmdesigner.appspot.com/](http://jqmdesigner.appspot.com/)




