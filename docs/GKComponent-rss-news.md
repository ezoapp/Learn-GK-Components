##rss-news
Using `rss-news` of rss service, you can get easier access to updates about news topics that interest you.  

<br/>
###Properties
<table>

<tr>
<th style="background:#ddd;">property</th>
<th style="background:#ddd;">setting</th>
</tr>

<tr>
<td>id</td>
<td>Component's id</td>
</tr>

<tr>
<td>service</td>
<td>Rss service url</td>
</tr>

<tr>
<td>rowNum</td>
<td>Each page number of rows to be displayed</td>
</tr>

</table>

<br/>
###API
None

<br/>
###Javascript Code
After dragging the component into the design panel, in javascript editor panel, and it will generate the code ( `#componentId` is the component's id )：


	$(document).on("gkComponentsReady", function () {
	  var $ele = $("#componentId"),
	    FEED_URL = $ele.attr("service"),
	    $listview = $("#componentId").find('[data-role="listview"]');
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

EZoApp Official Site: [ezoui.com](http://ezoui.com/)  




