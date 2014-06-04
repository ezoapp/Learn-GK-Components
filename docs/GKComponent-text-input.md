##text-input
`text-input` 是文字輸入的元件，提供使用者單行的文字輸入，該元件拖曳進入設計區域後，預設與標題一起放在 `fieldcontain` 內，也可利用拖拉的方式將其移出 `fieldcontain` 外。

<br/>
###元件位置

以下列出 `text-input` 元件可以放置的位置，以及哪些元件可以放入 `text-input` 裡頭。
<table>
<tr>
<th style="background:#ddd;">位置說明</th>
<th style="background:#ddd;">相關元件</th>
</tr>
<tr>
<td>text-input 可以放在哪些元件內？
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
<td>哪些元件可以放在 text-input 內？</td>
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
<td>name</td>
<td>名稱</td>
</tr>

<tr>
<td>value</td>
<td>回傳值</td>
</tr>

<tr>
<td>style</td>
<td>直接編寫元件 DOM inline 樣式</td>
</tr>

<tr>
<td>placeholder</td>
<td>預顯示文字</td>
</tr>

<tr>
<td>clearBtn</td>
<td>
<ul>
<li>true：輸入時出現清除按鈕</li>
<li>false：輸入時隱藏清除按鈕</li>
</ul></td>
</tr>

<tr>
<td>clearBtnText</td>
<td>清除按鈕的說明文字</td>
</tr>

<tr>
<td>mini</td>
<td><ul>
<li>true：最小化</li>
<li>false：正常尺寸</li>
</ul></td>
</tr>

<tr>
<td>disable</td>
<td><ul>
<li>(default)：預設顯示可使用</li>
<li>disable：顯示但不可使用</li>
</ul></td>
</tr>

<tr>
<td>preventFocusZoom</td>
<td><ul>
<li>true：</li>
<li>false：</li>
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
<td>isUseGKComponent</td>
<td><ul>
<li>true：轉換為 GK 元件 ( 可使用 GK 元件 API )a</li>
<li>false：不轉換為 GK 元件</li>
</ul></td>
</tr>

</table>
<br/>
###API
若已由 `isUseGKComponent` 將元件轉換為 GK 元件，則可使用 GK 元件之 API，使用方式就是在元件 id 後方加上 `.gk()`，後方接上 API 名稱即可使用，以下範例使用 id 為 test 的 `text-input` 元件。

- **value**：  
  	> 描述。

			$('#test').gk().value();


<br/>
----------
以上便是 `text-input` 的相關說明，如果想了解更多其他元件，請回 [元件清單列表](https://github.com/ezoapp/Learn-GK-Components)  

官方網站：[www.ezoui.com/app](http://www.ezoui.com/app)  
EZoApp 開發工具：[jqmdesigner.appspot.com/](http://jqmdesigner.appspot.com/)




