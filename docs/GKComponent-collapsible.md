##collapsible
`collapsible` 是點選標題的按鈕之後，進行內容收合或展開的元件。

<br/>
###元件位置
以下列出 `collapsible` 元件可以放置的位置，以及哪些元件可以放入 `collapsible` 裡頭。
<table>
<tr>
<th style="background:#ddd;">位置說明</th>
<th style="background:#ddd;">相關元件</th>
</tr>
<tr>
<td>collapsible 可以放在哪些元件內？
</td>
<td>
<ul>
<li>collapsible-set</li>
<li>collapsible</li>
</ul>
</td>
</tr>
<tr>
<td>哪些元件可以放在 collapsible 內？</td>
<td>所有元件均可放入 ( 除了 header 和 footer )</td>
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
<td></td>
</tr>

<tr>
<td>collapsed</td>
<td></td>
</tr>

<tr>
<td>iconPos</td>
<td><ul>
<li>left：icon 在左側</li>
<li>right：icon 在左右側</li>
<li>bottom：icon 在下</li>
<li>top：icon 在上</li>
<li>notnext：不要文字，只有 icon</li>
</ul></td>
</tr>

<tr>
<td>collapsedIcon</td>
<td></td>
</tr>

<tr>
<td>expandedIcon</td>
<td></td>
</tr>

<tr>
<td>inset</td>
<td></td>
</tr>

<tr>
<td>mini</td>
<td><ul>
<li>true：最小化</li>
<li>false：正常尺寸</li>
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
<td>content theme</td>
<td><ul>
<li>a：內容樣式 a</li>
<li>b：內容樣式 b</li>
</ul></td>
</tr>

<tr>
<td>isUseGKComponent</td>
<td><ul>
<li>true：轉換為 GK 元件 ( 可使用 GK 元件 API )</li>
<li>false：不轉換為 GK 元件</li>
</ul></td>
</tr>

</table>

<br/>
###API
若已由 `isUseGKComponent` 將元件轉換為 GK 元件，則可使用 GK 元件之 API，使用方式就是在元件 id 後方加上 `.gk()`，後方接上 API 名稱即可使用，以下範例使用 id 為 test 的 `collapsible` 元件。

- **expand**：  
  	> 描述。

			$('#test').gk().expand();

- **collapse**：  
  	> 描述。

			$('#test').gk().collapse();


<br/>
----------
以上便是 `collapsible` 的相關說明，如果想了解更多其他元件，請回 [元件清單列表](https://github.com/ezoapp/Learn-GK-Components)  

官方網站：[www.ezoui.com/app](http://www.ezoui.com/app)  
EZoApp 開發工具：[jqmdesigner.appspot.com/](http://jqmdesigner.appspot.com/)




