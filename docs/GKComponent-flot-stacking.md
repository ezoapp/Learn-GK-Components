##flot-stacking
`flot-stacking` 可以協助使用者產生 stacking 的圖表，採用 flot-stacking 的樣式。 

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
Above is the description of `flot-stacking`. For more information, please back to [GK-Components-List](https://github.com/ezoapp/Learn-GK-Components).

Offical Site：[www.ezoui.com/app/](http://www.ezoui.com/app/)  
EZoApp Designer：[jqmdesigner.appspot.com/](http://jqmdesigner.appspot.com/)




