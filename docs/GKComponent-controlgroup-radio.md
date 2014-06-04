##controlgroup-radio
`controlgroup-radio` 元件提供使用者「單選」的按鈕，是由 `radio-button` 與 `controlgroup` 所組成，也可參考 [radio-button 元件說明](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-radio-button.md)

<br/>
###元件位置
以下列出 `controlgroup-radio` 元件可以放置的位置，以及哪些元件可以放入 `controlgroup-radio` 裡頭。
<table>
<tr>
<th style="background:#ddd;">位置說明</th>
<th style="background:#ddd;">相關元件</th>
</tr>
<tr>
<td>controlgroup-radio 可以放在哪些元件內？
</td>
<td>
<ul>
<li>page</li>
<li>header</li>
<li>footer</li>
<li>content</li>
<li>block</li>
<li>collapsible-set</li>
<li>collapsible</li>
<li>listview-li</li>
</ul>
</td>
</tr>
<tr>
<td>哪些元件可以放在 controlgroup-radio 內？</td>
<td>
<ul>
<li>radio-button</li>
<li>raty</li>
</ul>
</td>
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
<td>class</td>
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
<td>types</td>
<td></td>
</tr>

<tr>
<td>iconPos</td>
<td></td>
</tr>

<tr>
<td>corners</td>
<td></td>
</tr>

<tr>
<td>mini</td>
<td></td>
</tr>

<tr>
<td>shadow</td>
<td></td>
</tr>

<tr>
<td>excludeInvisible</td>
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
若已由 `isUseGKComponent` 將元件轉換為 GK 元件，則可使用 GK 元件之 API，使用方式就是在元件 id 後方加上 `.gk()`，後方接上 API 名稱即可使用，以下範例使用 id 為 test 的 `controlgroup-radio` 元件。

- **model**：  
  	> 描述。

			$('#test').gk().model();

- **apply**：  
  	> 描述。

			$('#test').gk().apply();

- **checked**：  
  	> 描述。

			$('#test').gk().checked();

- **unchecked**：  
  	> 描述。

			$('#test').gk().unchecked();

- **onSelect**：  
  	> 描述。

			$('#test').gk().onSelect();

- **disable**：  
  	> 描述。

			$('#test').gk().disable();

- **enable**：  
  	> 描述。

			$('#test').gk().enable();
<br/>
----------
以上便是 `controlgroup-radio` 的相關說明，如果想了解更多其他元件，請回 [元件清單列表](https://github.com/ezoapp/Learn-GK-Components)  

官方網站：[www.ezoui.com/app](http://www.ezoui.com/app)  
EZoApp 開發工具：[jqmdesigner.appspot.com/](http://jqmdesigner.appspot.com/)




