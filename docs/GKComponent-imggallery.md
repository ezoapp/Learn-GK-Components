##imggallery
`imggallery` 元件可以獲取 flickr 中的照片，再根據使用者的樣式設定進行相簿的排版 

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
<td>width</td>
<td></td>
</tr>

<tr>
<td>image-Height</td>
<td></td>
</tr>

<tr>
<td>image-Width</td>
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
若已由 `isUseGKComponent` 將元件轉換為 GK 元件，則可使用 GK 元件之 API，使用方式就是在元件 id 後方加上 `.gk()`，後方接上 API 名稱即可使用，以下範例使用 id 為 test 的 `imggallery` 元件。

- **onclick**：  
  	> 描述。

			$('#test').gk().onclick();


- **model**：  
  	> 描述。

			$('#test').gk().model();

<br/>
###Javascript 面板內容
元件拖拉進入設計區域後，會在 javascript 的編輯面板同步產生下列代碼：

	$(document).on("gkComponentsReady", function (w) {
	  var img = [{
	    "data-src": "http://www.dropmysite.com/images/social/icon-google.png?1386321977"
	  }, {
	    "data-src": "http://www.dropmysite.com/images/social/icon-facebook.png?1386321977"
	  }, {
	    "data-src": "http://www.dropmyemail.com/assets/icon-twitter-963acb3e091cfea4ef6394d6c3b9e388.png"
	  }];
	  $("#gk-6470VT").gk("model", img);
	  $("#gk-6470VT").gk("onclick", function (e) {
	    alert(e.target);
	  });
	});

<br/>
----------
Above is the description of `imggallery`. For more information, please back to [GK-Components-List](https://github.com/ezoapp/Learn-GK-Components).

Offical Site：[www.ezoui.com/app/](http://www.ezoui.com/app/)  
EZoApp Designer：[jqmdesigner.appspot.com/](http://jqmdesigner.appspot.com/)




