##imggallery
`imggallery` can get flickr photos, and then the album layout based on the user's style settings 

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

</table>

<br/>
###API

- **onclick**：  
  	> description

			$('#test').gk().onclick();


- **model**：  
  	> description

			$('#test').gk().model();

<br/>
###Javascript Code
After dragging the component into the design panel, in javascript editor panel, and it will generate the code ( `#componentId` is the component's id )：

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




