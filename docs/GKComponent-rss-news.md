##rss-news
`rss-news` 可以將公開資訊的 rss 資料，以清單列表的方式呈現於畫面當中。  


<br/>
###元件位置
以下列出 `rss-news` 元件可以放置的位置，以及哪些元件可以放入 `rss-news` 裡頭。
<table>
<tr>
<th style="background:#ddd;">位置說明</th>
<th style="background:#ddd;">相關元件</th>
</tr>
<tr>
<td>rss-news 可以放在哪些元件內？
</td>
<td>
<ul>
<li>page</li>
<li>header</li>
<li>footer</li>
<li>content</li>
<li>block</li>
<li>collapsible</li>
<li>controlgroup</li>
</ul>
</td>
</tr>
<tr>
<td>哪些元件可以放在 rss-news 內？</td>
<td>無</td>
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
<td>isUseGKComponent</td>
<td><ul>
<li>true：轉換為 GK 元件 ( 可使用 GK 元件 API )a</li>
<li>false：不轉換為 GK 元件</li>
</ul></td>
</tr>

<tr>
<td>rowNum</td>
<td></td>
</tr>

<tr>
<td>service</td>
<td></td>
</tr>

</table>

<br/>
###API
`rss-news` 元件沒有提供 api。

<br/>
###Javascript 面板內容
元件拖拉進入設計區域後，會在 javascript 的編輯面板同步產生下列代碼：


	$(document).on("gkComponentsReady", function () {
	  var $ele = $("元件id"),
	    FEED_URL = $ele.attr("service"),
	    $listview = $("元件id").find('[data-role="listview"]');
	  rowNum = $ele.attr('rowNum');
	
	  if (FEED_URL) {
	    $.ajax({
	      beforeSend: function () {
	        $listview.css('visibility', 'hidden');
	      },
	      url: 'http://ajax.googleapis.com/ajax/services/feed/load?v=1.0&num=' + rowNum + '&callback=?&q=' + encodeURIComponent(FEED_URL),
	      dataType: 'json',
	      success: function (data) {
	        if (data.responseData.feed && data.responseData.feed.entries) {
	          var models = data.responseData.feed.entries;
	          $listview.gk('model', models);
	          $listview.css('visibility', 'visible');
	        }
	      }
	    });
	  }
	
	  $listview.gk('onRow', function (vo) {
	    alert(JSON.stringify(vo));
	  });
	
	});


<br/>
----------
以上便是 `rss-news` 的相關說明，如果想了解更多其他元件，請回 [元件清單列表](https://github.com/ezoapp/Learn-GK-Components)  

官方網站：[www.ezoui.com/app](http://www.ezoui.com/app)  
EZoApp 開發工具：[jqmdesigner.appspot.com/](http://jqmdesigner.appspot.com/)




