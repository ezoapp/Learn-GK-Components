#GK Component - header#

`header` 元件會固定在畫面的頂端，主要用來顯示固定的頁面標題或按鈕。  

##元件位置##

以下列出 `header` 元件可以放置的位置，以及哪些元件可以放入 `header` 裡頭。
<table>
<tr>
<th style="background:#ddd;">元件位置說明</th>
<th style="background:#ddd;">元件</th>
</tr>
<tr>
<td>header 可以放在哪些元件內？
</td>
<td>無，header 只能放在 Page 裡</td>
</tr>
<tr>
<td>哪些元件可以放在 header 內？</td>
<td>所有元件均可放在 header 內</td>
</tr>
</table>

##屬性設定##

- **id**  
  元件的 id
- **text**  
  元件的顯示文字
- **style**  
  直接編寫元件 DOM inline 樣式
- **position**  
	- default：隨畫面移動
	- fixed：固定在最上方
- **fullscreen** ( position = fixed 時才會出現 )
	- true：瀏覽時 header 消失，點選畫面後 header 顯示
	- false：header 永遠顯示
- **theme**
	- a：樣式 a
	- b：樣式 b
- **isUseGKComponent**
	- true：轉換為 GK 元件 ( 可使用 GK 元件 API )
	- false：不轉換為 GK 元件

##API##
若已由 `isUseGKComponent` 將元件轉換為 GK 元件，則可使用 GK 元件之 API，使用方式就是在元件 id 後方加上 `.gk()`，後方接上 API 名稱即可使用。  

- **label**：  
  *置換 header 內容文字，下列範例將 header 置換為 test header。*

		$(document).on('gkComponentsReady', function () {
			$('#test').gk().label('test header');
		});





