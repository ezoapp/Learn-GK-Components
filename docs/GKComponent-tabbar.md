##tabbar
`tabbar` 元件是固定置底的按鈕元件，本質上其實是 `navbar` 與 `footer` 的組合，因此相關的位置、設定與 API ，和 `navbar` 元件是相同的，可參考 [navbar 元件說明](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-navbar.md)。  

<br/>
###元件位置

以下列出 `tabbar` 元件可以放置的位置，以及哪些元件可以放入 `tabbar` 裡頭。
<table>
<tr>
<th style="background:#ddd;">位置說明</th>
<th style="background:#ddd;">相關元件</th>
</tr>
<tr>
<td>tabbar 可以放在哪些元件內？
</td>
<td>無，tabbar 只能放在 Page 裡</td>
</tr>
<tr>
<td>哪些元件可以放在 tabbar 內？</td>
<td>navbtn</td>
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
<td>style</td>
<td>直接編寫元件 DOM inline 樣式</td>
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
<td>transition</td>
<td><ul>
<li>slide：頁面左右滑動效果</li>
<li>slideup：頁面往上滑動</li>
<li>slidedown：頁面往下滑動</li>
<li>slidefade：頁面滑動+淡入</li>
<li>pop：彈出式頁面</li>
<li>fade：頁面淡入</li>
<li>flip：翻頁效果</li>
<li>flow：輸送帶效果</li>
<li>turn：旋轉效果</li>
<li>none：無效果</li>
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

<br/>
###API
`tabbar` 元件沒有提供 api。


<br/>
----------
以上便是 `tabbar` 的相關說明，如果想了解更多其他元件，請回 [元件清單列表](https://github.com/ezoapp/Learn-GK-Components)  

官方網站：[www.ezoui.com/app](http://www.ezoui.com/app)  
EZoApp 開發工具：[jqmdesigner.appspot.com/](http://jqmdesigner.appspot.com/)




