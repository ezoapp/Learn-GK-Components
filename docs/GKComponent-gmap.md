#gmap
`gmap` 元件可讓使用者藉由設定的方式，完成 Google map 的顯示  


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
<td>zoom</td>
<td></td>
</tr>

<tr>
<td>address</td>
<td></td>
</tr>

<tr>
<td>mapTypeId</td>
<td></td>
</tr>

<tr>
<td>markerTitle</td>
<td></td>
</tr>

<tr>
<td>latitude</td>
<td></td>
</tr>

<tr>
<td>longitude</td>
<td></td>
</tr>

</table>

<br/>
###API
若已由 `isUseGKComponent` 將元件轉換為 GK 元件，則可使用 GK 元件之 API，使用方式就是在元件 id 後方加上 `.gk()`，後方接上 API 名稱即可使用，以下範例使用 id 為 test 的 `gmap` 元件。

- **height**：  
  	> 描述。

			$('#test').gk().height();


- **width**：  
  	> 描述。

			$('#test').gk().width();


- **nowPos**：  
  	> 描述。

			$('#test').gk().nowPos();


- **location**：  
  	> 描述。

			$('#test').gk().location();


- **zoom**：  
  	> 描述。

			$('#test').gk().zoom();


- **address**：  
  	> 描述。

			$('#test').gk().address();


- **markerTitle**：  
  	> 描述。

			$('#test').gk().markerTitle();


<br/>
----------
Above is the description of `gmap`. For more information, please back to [GK-Components-List](https://github.com/ezoapp/Learn-GK-Components).

Offical Site：[www.ezoui.com/app/](http://www.ezoui.com/app/)  
EZoApp Designer：[jqmdesigner.appspot.com/](http://jqmdesigner.appspot.com/)



