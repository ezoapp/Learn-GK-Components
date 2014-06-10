##page-listview
`page-listview` allows us the information, presented in a way to list 

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

<tr>
<td>style</td>
<td>HTML inline style</td>
</tr>

<tr>
<td>pageSize</td>
<td>Count each page</td>
</tr>

<tr>
<td>url</td>
<td>Data url</td>
</tr>

</table>

<br/>
###API

- **onRow(callback))**：  
  	> When you click on listview item , onRow will be invoke.
    > First argument of callback is JSON Object.

          $('#listview').gk().onRow(function(vo) {

          });

- **refresh**：  
 	> If you call remote API to set data , you must call the refresh method on it to update the visual styling.

		$('#listview').gk().refresh();


- **pageSize**：  
  	> description

			$('#test').gk().onRow();


- **remote**：  
  	> description

			$('#test').gk().onRow();


<br/>
----------
Above is the description of `page-listview`. For more information, please back to [GK-Components-List](https://github.com/ezoapp/Learn-GK-Components).

Offical Site：[www.ezoui.com/app/](http://www.ezoui.com/app/)  
EZoApp Designer：[jqmdesigner.appspot.com/](http://jqmdesigner.appspot.com/)




