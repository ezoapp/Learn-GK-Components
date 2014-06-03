#GK Component - youtube#

`youtube` 元件描述  

##元件位置##

以下列出 `youtube` 元件可以放置的位置，以及哪些元件可以放入 `youtube` 裡頭。
<table>
<tr>
<th style="background:#ddd;">位置說明</th>
<th style="background:#ddd;">相關元件</th>
</tr>
<tr>
<td>youtube 可以放在哪些元件內？
</td>
<td></td>
</tr>
<tr>
<td>哪些元件可以放在 youtube 內？</td>
<td></td>
</tr>
</table>

##屬性設定##
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
<td>position</td>
<td><ul>
<li>default：隨畫面移動</li>
<li>fixed：固定在最上方</li>
</ul></td>
</tr>

<tr>
<td>fullscreen</td>
<td>
( position = fixed 時才會出現 )
<ul>
<li>true：瀏覽時 header 消失，點選畫面後 header 顯示</li>
<li>false：header 永遠顯示</li>
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
<td>isUseGKComponent</td>
<td><ul>
<li>true：轉換為 GK 元件 ( 可使用 GK 元件 API )a</li>
<li>false：不轉換為 GK 元件</li>
</ul></td>
</tr>

</table>

##API##
若已由 `isUseGKComponent` 將元件轉換為 GK 元件，則可使用 GK 元件之 API，使用方式就是在元件 id 後方加上 `.gk()`，後方接上 API 名稱即可使用，以下範例使用 id 為 test 的 `youtube` 元件。

- **api**：  
  	> 描述。

			程式碼


<br/>
----------
以上便是 `youtube` 的相關說明，如果想了解更多其他元件，請回 [元件清單列表](https://github.com/ezoapp/Learn-GK-Components)  

官方網站：[www.ezoui.com/app](http://www.ezoui.com/app)  
EZoApp 開發工具：[jqmdesigner.appspot.com/](http://jqmdesigner.appspot.com/)




