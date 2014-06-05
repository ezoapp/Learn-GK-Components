##flot-line
`flot-line` 會由使用者在 javascript 中的陣列，產生對應的線狀圖表，圖表樣式採用 `flot-line`的樣式呈現。

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
<td>class</td>
<td></td>
</tr>

<tr>
<td>style</td>
<td></td>
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
<td>showPoints</td>
<td></td>
</tr>

<tr>
<td>showLabels</td>
<td></td>
</tr>

<tr>
<td>labelPlacement</td>
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
None


<br/>
###Javascript 面板內容
元件拖拉進入設計區域後，會在 javascript 的編輯面板同步產生下列代碼：  

	$(document).on("gkComponentsReady", function () {
	  var dataset_tv = {
	    data: [
	      [1, 45],
	      [2, 44],
	      [3, 43],
	      [4, 42],
	      [5, 38]
	    ],
	    label: 'TV'
	  };
	
	  var dataset_online = {
	    data: [
	      [1, 25],
	      [2, 26],
	      [3, 26],
	      [4, 26],
	      [5, 20]
	    ],
	    label: 'Online'
	  };
	
	  var dataset_radio = {
	    data: [
	      [1, 17],
	      [2, 16],
	      [3, 15],
	      [4, 14],
	      [5, 12]
	    ],
	    label: 'Radio',
	    color: '#469a54'
	  };
	
	  var dataset_mobile = {
	    data: [
	      [1, 4],
	      [2, 6],
	      [3, 9],
	      [4, 12],
	      [5, 20]
	    ],
	    label: 'Mobile',
	    labels: ["4%", "6%", "9%", "12%", "20%"]
	  };
	
	  var options = {
	    xaxis: {
	      autoscaleMargin: 0.5,
	      ticks: [
	        [1, 2009],
	        [2, 2010],
	        [3, 2011],
	        [4, 2012],
	        [5, 2013]
	      ]
	    }
	  };
	
	  $('#gk-64wHYf').gk('render', [dataset_tv, dataset_online, dataset_radio, dataset_mobile], options);
	});


<br/>
----------
Above is the description of `flot-line`. For more information, please back to [GK-Components-List](https://github.com/ezoapp/Learn-GK-Components).

Offical Site：[www.ezoui.com/app/](http://www.ezoui.com/app/)  
EZoApp Designer：[jqmdesigner.appspot.com/](http://jqmdesigner.appspot.com/)




