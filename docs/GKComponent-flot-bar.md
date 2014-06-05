##flot-bar
`flot-bar` 可以協助使用者產生 bar 的圖表，採用 flot-bar 的樣式。   

<br/>
###Properties
<table>

<tr>
<th style="background:#ddd;">property</th>
<th style="background:#ddd;">setting</th>
</tr>

<tr>
<td>id</td>
<td>元件Component's id</td>
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
Above is the description of `flot-bar`. For more information, please back to [GK-Components-List](https://github.com/ezoapp/Learn-GK-Components).

Offical Site：[www.ezoui.com/app/](http://www.ezoui.com/app/)  
EZoApp Designer：[jqmdesigner.appspot.com/](http://jqmdesigner.appspot.com/)




