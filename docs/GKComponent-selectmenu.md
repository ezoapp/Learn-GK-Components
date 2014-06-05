##selectmenu
`selectmenu` 可以利用點選的方式，讓使用者展開選單進行連結或切換頁，該元件拖曳進入設計區域後，預設與標題一起放在 `fieldcontain` 內，也可利用拖拉的方式將其移出 `fieldcontain` 外。  

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
<td>name</td>
<td></td>
</tr>

<tr>
<td>inline</td>
<td></td>
</tr>

<tr>
<td>nativeMenu</td>
<td></td>
</tr>

<tr>
<td>icon</td>
<td></td>
</tr>

<tr>
<td>iconPos</td>
<td></td>
</tr>

<tr>
<td>iconshadow</td>
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
<td>disable</td>
<td></td>
</tr>

<tr>
<td>shadow</td>
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
若已由 `isUseGKComponent` 將元件轉換為 GK 元件，則可使用 GK 元件之 API，使用方式就是在元件 id 後方加上 `.gk()`，後方接上 API 名稱即可使用，以下範例使用 id 為 test 的 `selectmenu` 元件。

- **value**：  
  	> 描述。

			$('#test').gk().value();

- **enable**：  
  	> 描述。

			$('#test').gk().enable();

- **disable**：  
  	> 描述。

			$('#test').gk().disable();

- **open**：  
  	> 描述。

			$('#test').gk().open();

- **close**：  
  	> 描述。

			$('#test').gk().close();

- **refresh**：  
  	> 描述。

			$('#test').gk().value();


- **model**：  
  	> 描述。

			$('#test').gk().value();


- **onChange**：  
  	> 描述。

			$('#test').gk().value();


<br/>
----------
Above is the description of `selectmenu`. For more information, please back to [GK-Components-List](https://github.com/ezoapp/Learn-GK-Components).

Offical Site：[www.ezoui.com/app/](http://www.ezoui.com/app/)  
EZoApp Designer：[jqmdesigner.appspot.com/](http://jqmdesigner.appspot.com/)




