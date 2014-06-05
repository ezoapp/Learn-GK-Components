##json-listview
`json-listview` 元件可以讀入 json 的檔案，在以清單條列式的方式顯示。 

<br/>
###Properties
<table>

<tr>
<th style="background:#ddd;">property</th>
<th style="background:#ddd;">setting</th>
</tr>

<tr>
<td>id</td>
<td>component's id</td>
</tr>

</table>

<br/>
###API###

- **refresh**：  
  	> 描述。

			$('#test').gk().onRow();


- **onRow**：  
  	> 描述。

			$('#test').gk().onRow();


- **model**：  
  	> 描述。

			$('#test').gk().onRow();


- **apply**：  
  	> 描述。

			$('#test').gk().onRow();


<br/>
###Javascript 面板內容
元件拖拉進入設計區域後，會在 javascript 的編輯面板同步產生下列代碼：

	$(document).on("pageinit", "#home", function () {
	  var $ele = $("#gk-64HnU8"),
	    url = $ele.attr("service");
	  if (url) {
	    $.getJSON(url).complete(function (data) {
	      $("#gk-64HnU8").gk("model", $.parseJSON(data.responseText));
	    });
	  }
	});

<br/>
----------
Above is the description of `json-listview`. For more information, please back to [GK-Components-List](https://github.com/ezoapp/Learn-GK-Components).

Offical Site：[www.ezoui.com/app/](http://www.ezoui.com/app/)  
EZoApp Designer：[jqmdesigner.appspot.com/](http://jqmdesigner.appspot.com/)





