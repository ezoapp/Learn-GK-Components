##json-listview
`json-listview` can be read into json files to the list displayed.

<br/>
###Properties
Refer to JQueryMobile's [listview](http://api.jquerymobile.com/listview/) Widget.

<br/>
###API

- **refresh**：  
 	> If you set data to listview via JavaScript , you must call the refresh method on it to update the visual styling.

		$('#listview').gk().refresh();

- **onRow(callback))**：  
  	> When you click on listview item , onRow will be invoke.
    > If set data by model API , first argument of callback is JSON Object.
    > If set data by apply API , first argument of callback is li element of JQuery.

          // If call model API , callback argument is value object
          $('#listview').gk().model(data);
          $('#listview').gk().onRow(function(vo) {

          });

          // If call apply API , callback argument is li element of JQuery
          $('#listview').gk().apply(data);
          $('#listview').gk().onRow(function($li) {

          });    

- **model**：  
  	> Set data to listview , data type is JSON Array.
            
          var data = [{
            userId: '001',
            userName: 'Keven'
          }, {
            userId: '002',
            userName: 'Joe'
          }];

          $('#listview').gk().model(data);
          
  	> HTML template pattern {{ data.key }}
  	
        <li divider="{{userId}}" is="listview-li">
        	<span >{{userName}}</span>
        </li>             

- **apply**：  
  	> Set data to listview when data is only one , data type is JSON Object

          var data = {
            userId: '001',
            userName: 'Keven'
          };

          $('#listview').gk().model(apply);
          
  	> HTML template pattern {{data.key}}
  	
        <li divider="{{userId}}" is="listview-li">
        	<span >{{userName}}</span>
        </li>          
<br/>
###Javascript Code
After dragging the component into the design panel, in javascript editor panel, and it will generate the code ( `#componentId` is the component's id )：

		  var url = "open service url";
		  if (url) {
		    $.getJSON(url).complete(function (data) {
		      $("#listview").gk().model($.parseJSON(data.responseText));
		    });
		  }

<br/>
----------
Above is the description of `json-listview`. For more information, please back to [GK-Components-List](https://github.com/ezoapp/Learn-GK-Components).

Offical Site：[www.ezoui.com/app/](http://www.ezoui.com/app/)  
EZoApp Designer：[jqmdesigner.appspot.com/](http://jqmdesigner.appspot.com/)





