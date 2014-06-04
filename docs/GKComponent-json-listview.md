##json-listview
`json-listview` 元件可以讀入 json 的檔案，在以清單條列式的方式顯示。 

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
<td>style</td>
<td>直接編寫元件 DOM inline 樣式</td>
</tr>

<tr>
<td>inset</td>
<td></td>
</tr>

<tr>
<td>icon</td>
<td></td>
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
<td>autodividers</td>
<td></td>
</tr>

<tr>
<td>filter</td>
<td></td>
</tr>

<tr>
<td>divider theme</td>
<td></td>
</tr>

<tr>
<td>countTheme</td>
<td></td>
</tr>

<tr>
<td>theme</td>
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
###API###
若已由 `isUseGKComponent` 將元件轉換為 GK 元件，則可使用 GK 元件之 API，使用方式就是在元件 id 後方加上 `.gk()`，後方接上 API 名稱即可使用，以下範例使用 id 為 test 的 `json-listview` 元件。

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
以上便是 `json-listview` 的相關說明，如果想了解更多其他元件，請回 [元件清單列表](https://github.com/ezoapp/Learn-GK-Components)  

官方網站：[www.ezoui.com/app](http://www.ezoui.com/app)  
EZoApp 開發工具：[jqmdesigner.appspot.com/](http://jqmdesigner.appspot.com/)




