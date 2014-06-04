##bxslider
`bxslider` 是一個圖片輪播的元件，除了會自動輪播，使用者也可以用滑動或點選的方式進行圖片的切換。  

<br/>
###元件位置
以下列出 `bxslider` 元件可以放置的位置，以及哪些元件可以放入 `bxslider` 裡頭。
<table>
<tr>
<th style="background:#ddd;">位置說明</th>
<th style="background:#ddd;">相關元件</th>
</tr>
<tr>
<td>bxslider 可以放在哪些元件內？
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
<li>list-divider</li>
</ul>
</td>
</tr>
<tr>
<td>哪些元件可以放在 bxslider 內？</td>
<td></td>
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

</table>

<br/>
###API
`bxslider` 元件沒有提供 api。

<br/>
###Javascript 面板內容
元件拖拉進入設計區域後，會在 javascript 的編輯面板同步產生下列代碼：

	$(document).on("pageshow", function () {
	  /* Powered by http://bxslider.com/ */
	  $(".bxslider").bxSlider();
	});

<br/>
----------
以上便是 `bxslider` 的相關說明，如果想了解更多其他元件，請回 [元件清單列表](https://github.com/ezoapp/Learn-GK-Components)  

官方網站：[www.ezoui.com/app](http://www.ezoui.com/app)  
EZoApp 開發工具：[jqmdesigner.appspot.com/](http://jqmdesigner.appspot.com/)




