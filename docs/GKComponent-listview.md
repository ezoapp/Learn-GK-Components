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
<td>元件的 id</td>
</tr>

<tr>
<td>style</td>
<td>直接編寫元件 DOM inline 樣式</td>
</tr>

<tr>
<td>class</td>
<td>新增 class 樣式</td>
</tr>

<tr>
<td>order list</td>
<td><ul>
<li>true：清單顯示數字</li>
<li>false：清單隱藏數字</li>
</ul></td>
</tr>

<tr>
<td>readonly</td>
<td><ul>
<li>true：不能點選,純粹清單顯示</li>
<li>false：可以點選，進行切換或連結</li>
</ul></td>
</tr>

<tr>
<td>inset</td>
<td><ul>
<li>true：listview 可以出現在本文中間，四個角會有圓弧形</li>
<li>false：不出現在本文中間</li>
</ul></td>
</tr>

<tr>
<td>filter</td>
<td><ul>
<li>true：出現搜尋框篩選器，可搜尋清單內容</li>
<li>false：隱藏搜尋框篩選器</li>
</ul></td>
</tr>

<tr>
<td>theme</td>
<td><ul>
<li>a：樣式 a</li>
<li>b：樣式 b</li>
</ul></td>
</tr>

<tr>
<td>icon</td>
<td>選擇對應的 icon 圖示</td>
</tr>

<tr>
<td>alt icon</td>
<td><ul>
<li>true：黑色的 icon ( 較適合淺色背景 )</li>
<li>false：白色的 icon ( 較適合深色背景 )</li>
</ul></td>
</tr>

<tr>
<td>auto dividers</td>
<td><ul>
<li>true：自動產生標題</li>
<li>false：使用自訂義標題</li>
</ul></td>
</tr>

<tr>
<td>divider theme</td>
<td><ul>
<li>a：樣式 a</li>
<li>b：樣式 b</li>
</ul></td>
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
若已由 `isUseGKComponent` 將元件轉換為 GK 元件，則可使用 GK 元件之 API，使用方式就是在元件 id 後方加上 `.gk()`，後方接上 API 名稱即可使用，以下範例使用 id 為 listview-test 的 `listview` 元件。

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






