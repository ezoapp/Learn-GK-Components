##gk-text
`gk-text` 是標題或文字的元件，也可藉由傳值的方式動態產生相對應的文字。  

<br/>
###元件位置
以下列出 `gk-text` 元件可以放置的位置，以及哪些元件可以放入 `gk-text` 裡頭。
<table>
<tr>
<th style="background:#ddd;">位置說明</th>
<th style="background:#ddd;">相關元件</th>
</tr>
<tr>
<td>gk-text 可以放在哪些元件內？
</td>
<td>
<ul>
<li>page</li>
<li>header</li>
<li>footer</li>
<li>content</li>
<li>block</li>
<li>listview-li</li>
<li>collapsible</li>
<li>controlgroup</li>
<li>fieldcontain</li>
</ul>
</td>
</tr>
<tr>
<td>哪些元件可以放在 gk-text 內？</td>
<td>無</td>
</tr>
</table>

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
<td>text</td>
<td>元件的顯示文字</td>
</tr>

<tr>
<td>style</td>
<td>直接編寫元件 DOM inline 樣式</td>
</tr>

<tr>
<td>text type</td>
<td>可選擇 h1 ~ h6 的字體大小</td>
</tr>

</table>

<br/>
###API
若已由 `isUseGKComponent` 將元件轉換為 GK 元件，則可使用 GK 元件之 API，使用方式就是在元件 id 後方加上 `.gk()`，後方接上 API 名稱即可使用，以下範例使用 id 為 test 的 `gk-text` 元件。

- **text**：  
  	> 描述。

			$('#test').gk().text();


- **apply**：  
  	> 描述。

			$('#test').gk().apply();


<br/>
----------
以上便是 `gk-text` 的相關說明，如果想了解更多其他元件，請回 [元件清單列表](https://github.com/ezoapp/Learn-GK-Components)  

官方網站：[www.ezoui.com/app](http://www.ezoui.com/app)  
EZoApp 開發工具：[jqmdesigner.appspot.com/](http://jqmdesigner.appspot.com/)




