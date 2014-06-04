##textarea-input
`textarea-input` 是文字輸入的元件，提供使用者多行的文字輸入，該元件拖曳進入設計區域後，預設與標題一起放在 `fieldcontain` 內，也可利用拖拉的方式將其移出 `fieldcontain` 外。 

<br/>
###元件位置
以下列出 `textarea-input` 元件可以放置的位置，以及哪些元件可以放入 `textarea-input` 裡頭。
<table>
<tr>
<th style="background:#ddd;">位置說明</th>
<th style="background:#ddd;">相關元件</th>
</tr>
<tr>
<td>textarea-input 可以放在哪些元件內？
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
<li>fieldcontain</li>
</ul>
</td>
</tr>
<tr>
<td>哪些元件可以放在 textarea-input 內？</td>
<td></td>
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
<td>name</td>
<td></td>
</tr>

<tr>
<td>value</td>
<td></td>
</tr>

<tr>
<td>style</td>
<td>直接編寫元件 DOM inline 樣式</td>
</tr>

<tr>
<td>placeholder</td>
<td></td>
</tr>

<tr>
<td>autogrow</td>
<td></td>
</tr>

<tr>
<td>disabled</td>
<td></td>
</tr>

<tr>
<td>preventFocusZoom</td>
<td></td>
</tr>

<tr>
<td>theme</td>
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
若已由 `isUseGKComponent` 將元件轉換為 GK 元件，則可使用 GK 元件之 API，使用方式就是在元件 id 後方加上 `.gk()`，後方接上 API 名稱即可使用，以下範例使用 id 為 test 的 `textarea-input` 元件。

- **value**：  
  	> 描述。

			$('#test').gk().value();


<br/>
----------
以上便是 `textarea-input` 的相關說明，如果想了解更多其他元件，請回 [元件清單列表](https://github.com/ezoapp/Learn-GK-Components)  

官方網站：[www.ezoui.com/app](http://www.ezoui.com/app)  
EZoApp 開發工具：[jqmdesigner.appspot.com/](http://jqmdesigner.appspot.com/)




