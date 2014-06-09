##listview
A listview is coded as a simple unordered list containing linked list items with a `data-role="listview"` attribute.

<br/>
###Properties
Refer to JQueryMobile's [listview](http://api.jquerymobile.com/listview/) Widget.

<br/>
###API

- **refresh**：  
 	> refresh listview content

		$('#test-page').on('pageinit', function() {
		  $('#listview-test').gk().refresh();
		});

- **onRow**：  
  	> description

		  $('#listview-test').gk().onRow( _test);
		  function _test(){
		    alert('onRow');
		  }

- **model**：  
  	> description

		  $('#listview-test').gk().model();

- **apply**：  
  	> description

		  $('#listview-test').gk().apply();


<br/>
----------
Above is the description of `listview`. For more information, please back to [GK-Components-List](https://github.com/ezoapp/Learn-GK-Components).

Offical Site：[www.ezoui.com/app/](http://www.ezoui.com/app/)  
EZoApp Designer：[jqmdesigner.appspot.com/](http://jqmdesigner.appspot.com/)  






