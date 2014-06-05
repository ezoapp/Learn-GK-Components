##controlgroup-checkbox
`controlgroup-checkbox` 元件提供使用者「複選」的按鈕，是由 `checkbox-button` 與 `controlgroup` 所組成，也可參考 [checkbox-button 元件說明](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-checkbox-button.md) 

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
若已由 `isUseGKComponent` 將元件轉換為 GK 元件，則可使用 GK 元件之 API，使用方式就是在元件 id 後方加上 `.gk()`，後方接上 API 名稱即可使用，以下範例使用 id 為 test 的 `controlgroup-checkbox` 元件。

- **apply**：  
  	> 描述。

			$('#test').gk().apply();


- **onSelect**：  
  	> 描述。

			$('#test').gk().onSelect();


- **disable**：  
  	> 描述。

			$('#test').gk().disable();


- **enable**：  
  	> 描述。

			$('#test').gk().enable();


- **checked**：  
  	> 描述。

			$('#test').gk().checked();


- **unchecked**：  
  	> 描述。

			$('#test').gk().unchecked();



<br/>
----------
Above is the description of `controlgroup-checkbox`. For more information, please back to [GK-Components-List](https://github.com/ezoapp/Learn-GK-Components).

Offical Site：[www.ezoui.com/app/](http://www.ezoui.com/app/)  
EZoApp Designer：[jqmdesigner.appspot.com/](http://jqmdesigner.appspot.com/)




