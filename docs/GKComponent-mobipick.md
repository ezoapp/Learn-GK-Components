##mobipick
`mobipick` 元件在使用者點選後，會跳出翻頁效果的日期選擇清單，提供使用者選擇日期  


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
<td>value</td>
<td></td>
</tr>

<tr>
<td>style</td>
<td>直接編寫元件 DOM inline 樣式</td>
</tr>

<tr>
<td>min</td>
<td></td>
</tr>

<tr>
<td>max</td>
<td></td>
</tr>

<tr>
<td>accuracy</td>
<td></td>
</tr>

<tr>
<td>intlStdDate</td>
<td></td>
</tr>

<tr>
<td>dateFormat</td>
<td></td>
</tr>

<tr>
<td>dateFormatMonth</td>
<td></td>
</tr>

</table>

<br/>
###API
若已由 `isUseGKComponent` 將元件轉換為 GK 元件，則可使用 GK 元件之 API，使用方式就是在元件 id 後方加上 `.gk()`，後方接上 API 名稱即可使用，以下範例使用 id 為 test 的 `mobipick` 元件。

- **value**：  
  	> 描述。

			$('#test').gk().value();

- **getDateValue**：  
  	> 描述。

			$('#test').gk().getDateValue();

- **reset**：  
  	> 描述。

			$('#test').gk().reset();


<br/>
----------
Above is the description of `mobipick`. For more information, please back to [GK-Components-List](https://github.com/ezoapp/Learn-GK-Components).

Offical Site：[www.ezoui.com/app/](http://www.ezoui.com/app/)  
EZoApp Designer：[jqmdesigner.appspot.com/](http://jqmdesigner.appspot.com/)




