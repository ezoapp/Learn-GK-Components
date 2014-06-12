##page-listview
`page-listview` allows us by page to display data , you can decide to displayed record count on each page.  
Server side must be implement that get data by page count.


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
<td>style</td>
<td>HTML inline style</td>
</tr>

<tr>
<td>pageSize</td>
<td>Displayed record count on each page , minimum value is 30</td>
</tr>

<tr>
<td>url</td>
<td>Remote service url</td>
</tr>

</table>

Other properties , Please to refer to JQueryMobile's [listview](http://api.jquerymobile.com/listview/) Widget.
<br/>
###API

- **onRow(callback))**：  
  	> When you click on listview item , onRow will be invoke.  
	> First argument of callback is JSON Object.

          $('#listview').gk().onRow(function(vo) {

          });
  	> HTML template pattern {{ data.key }}
  	
        <li divider="{{userId}}" is="listview-li">
        	<span >{{userName}}</span>
        </li>             

- **refresh**：  
 	>  Call the refresh method on it to update the visual styling.

		$('#listview').gk().refresh();


- **pageSize(count)**：  
  	> Set displayed record count on each page.  
    > Get displayed record count on each page when count is null. 

		$('#listview').gk().pageSize();


- **remote(url , options)**：  
  	> Invoke remote service.  
  	> url argument is remote service url.  
  	> data argument is post extra data , type is JSON Object  

		$('#listview').gk().remote(url, data);

  	> Default post data for server side to implement thant get data by page
  	
  	    //For this example componentId is listview
        componentId.pagebar: {
          offset: 0     // Start index of current record
          pageSize: 30  // Record count on each page
        }    
<br/>
----------
Above is the description of `page-listview`. For more information, please back to [GK-Components-List](https://github.com/ezoapp/Learn-GK-Components).

Offical Site：[www.ezoui.com/app/](http://www.ezoui.com/app/)  
EZoApp Designer：[jqmdesigner.appspot.com/](http://jqmdesigner.appspot.com/)




