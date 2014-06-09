##listview
`listview` Display data in list , you can switch page or do action on click item .  
listview contains two component：[`list-divider`](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-list-divider.md)  ( header ) 、[`listview-li`](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-listview-li.md) ( item ) 

<br/>
###Properties
Refer to JQueryMobile's [listview](http://api.jquerymobile.com/listview/) Widget.

<br/>
###API

- **refresh**：  
 	> If you set data to listview via JavaScript , you must call the refresh method on it to update the visual styling.

		$('#listview-test').gk().refresh();

- **onRow(vo)**：  
  	> When you click on listview item , onRow will be invoke.

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






