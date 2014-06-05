##collapsible
`collapsible` 是點選標題的按鈕之後，進行內容收合或展開的元件。

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
Above is the description of `collapsible`. For more information, please back to [GK-Components-List](https://github.com/ezoapp/Learn-GK-Components).

Offical Site：[www.ezoui.com/app/](http://www.ezoui.com/app/)  
EZoApp Designer：[jqmdesigner.appspot.com/](http://jqmdesigner.appspot.com/)




