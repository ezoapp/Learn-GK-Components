##listview
`listview` 元件會以清單的方式顯示資料，並可在清單中進行連結和切換的動作，而 listview 裡頭又包含了兩個元件：`list-divider` ( 清單標題 ) 、`listview-li` ( 清單 )，可參考 [list-divider 元件說明](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-list-divider.md) 與 [listview-li 元件說明](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-listview-li.md)。

<br/>
###Properties
<table>

<tr>
<th style="background:#ddd;">property</th>
<th style="background:#ddd;">setting</th>
</tr>

<tr>
<td>id</td>
<td>Components id</td>
</tr>

<tr>
<td>style</td>
<td>HTML inline style</td>
</tr>

<tr>
<td>class</td>
<td>CSS class</td>
</tr>

<tr>
<td>order</td>
<td></td>
</tr>

<tr>
<td>readonly</td>
<td></td>
</tr>

<tr>
<td>data-inset</td>
<td></td>
</tr>

<tr>
<td>data-filter</td>
<td></td>
</tr>

<tr>
<td>data-filter-reveal</td>
<td></td>
</tr>

<tr>
<td>data-filter-placeholder</td>
<td></td>
</tr>

<tr>
<td>data-filter-theme</td>
<td></td>
</tr>

<tr>
<td>data-theme</td>
<td></td>
</tr>

<tr>
<td>data-icon</td>
<td></td>
</tr>

<tr>
<td>altIcon</td>
<td></td>
</tr>

<tr>
<td>data-autodividers</td>
<td></td>
</tr>

<tr>
<td>data-divider-theme</td>
<td></td>
</tr>

<tr>
<td>data-split-icon</td>
<td></td>
</tr>

<tr>
<td>data-split-theme</td>
<td></td>
</tr>

<tr>
<td>repeat</td>
<td></td>
</tr>

</table>

<br/>
###API

- **refresh**：  
 	> 刷新 listview 的內容

		$('#test-page').on('pageinit', function() {
		  $('#listview-test').gk().refresh();
		});

- **onRow**：  
  	> 點選整個 listview 時會觸發的事件

		  $('#listview-test').gk().onRow( _test);
		  function _test(){
		    alert('onRow');
		  }

- **model**：  
  	> model 描述

		  $('#listview-test').gk().model();

- **apply**：  
  	> apply 描述

		  $('#listview-test').gk().apply();


<br/>
----------
Above is the description of `listview`. For more information, please back to [GK-Components-List](https://github.com/ezoapp/Learn-GK-Components).

Offical Site：[www.ezoui.com/app/](http://www.ezoui.com/app/)  
EZoApp Designer：[jqmdesigner.appspot.com/](http://jqmdesigner.appspot.com/)  






