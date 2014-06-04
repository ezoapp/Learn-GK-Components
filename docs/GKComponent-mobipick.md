##mobipick
`mobipick` 元件在使用者點選後，會跳出翻頁效果的日期選擇清單，提供使用者選擇日期  


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
以上便是 `mobipick` 的相關說明，如果想了解更多其他元件，請回 [元件清單列表](https://github.com/ezoapp/Learn-GK-Components)  

官方網站：[www.ezoui.com/app](http://www.ezoui.com/app)  
EZoApp 開發工具：[jqmdesigner.appspot.com/](http://jqmdesigner.appspot.com/)




