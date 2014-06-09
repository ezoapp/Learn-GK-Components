##json-listview
`json-listview` can be read into json files to the list displayed.

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
  	> description

			$('#test').gk().onRow();


- **onRow**：  
  	> description

			$('#test').gk().onRow();


- **model**：  
  	> description

			$('#test').gk().onRow();


- **apply**：  
  	> description

			$('#test').gk().onRow();


<br/>
###Javascript Code
After dragging the component into the design panel, in javascript editor panel, and it will generate the code ( `#componentId` is the component's id )：

	$(document).on("pageinit", "#home", function () {
	  var $ele = $("#gk-64HnU8"),
	    url = $ele.attr("service");
	  if (url) {
	    $.getJSON(url).complete(function (data) {
	      $("#componentId").gk("model", $.parseJSON(data.responseText));
	    });
	  }
	});

<br/>
----------
Above is the description of `json-listview`. For more information, please back to [GK-Components-List](https://github.com/ezoapp/Learn-GK-Components).

Offical Site：[www.ezoui.com/app/](http://www.ezoui.com/app/)  
EZoApp Designer：[jqmdesigner.appspot.com/](http://jqmdesigner.appspot.com/)





