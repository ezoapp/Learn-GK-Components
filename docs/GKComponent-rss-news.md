##rss-news
`rss-news` 可以將公開資訊的 rss 資料，以清單列表的方式呈現於畫面當中。  

<br/>
###Properties
<table>

<tr>
<th style="background:#ddd;">property</th>
<th style="background:#ddd;">setting</th>
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
<td>一頁裡頭所呈現的資料筆數</td>
</tr>

<tr>
<td>service</td>
<td>rss 的網址</td>
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
Above is the description of `rss-news`. For more information, please back to [GK-Components-List](https://github.com/ezoapp/Learn-GK-Components).

Offical Site：[www.ezoui.com/app/](http://www.ezoui.com/app/)  
EZoApp Designer：[jqmdesigner.appspot.com/](http://jqmdesigner.appspot.com/)  




