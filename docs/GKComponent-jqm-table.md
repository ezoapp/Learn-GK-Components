##jqm-table
`jqm-table` 為一個表格元件，可以讓使用者點選自己想檢視的欄位進行檢視。

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

<tr>
<td>url</td>
<td></td>
</tr>

<tr>
<td>button text</td>
<td></td>
</tr>

<tr>
<td>stripe</td>
<td></td>
</tr>

<tr>
<td>stroke</td>
<td></td>
</tr>

<tr>
<td>shadow</td>
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
若已由 `isUseGKComponent` 將元件轉換為 GK 元件，則可使用 GK 元件之 API，使用方式就是在元件 id 後方加上 `.gk()`，後方接上 API 名稱即可使用，以下範例使用 id 為 test 的 `jqm-table` 元件。

- **load**：  
  	> 描述。

			$('#test').gk().load();


- **info**：  
  	> 描述。

			$('#test').gk().info();



<br/>
###Javascript 面板內容
元件拖拉進入設計區域後，會在 javascript 的編輯面板同步產生下列代碼：

	$(document).one("pageshow", "頁面id", function () {
	  var $ele = $("元件id"),
	    url = $ele.attr("loadURL");
	  if (url) {
	    $ele.gk("load", url);
	  }
	});



<br/>
----------
以上便是 `jqm-table` 的相關說明，如果想了解更多其他元件，請回 [元件清單列表](https://github.com/ezoapp/Learn-GK-Components)  

官方網站：[www.ezoui.com/app](http://www.ezoui.com/app)  
EZoApp 開發工具：[jqmdesigner.appspot.com/](http://jqmdesigner.appspot.com/)




