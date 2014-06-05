##flot-line
`flot-line` is plenty of options you can set to control the precise looks of your plot. You can control the ticks on the axes, the legend, the graph type, etc.

<br/>
###Properties
<table>

<tr>
<th style="background:#ddd;">property</th>
<th style="background:#ddd;">setting</th>
</tr>

<tr>
<td>id</td>
<td>component's id</td>
</tr>

<tr>
<td>class</td>
<td>CSS class</td>
</tr>

<tr>
<td>style</td>
<td>HTML inline style</td>
</tr>

</table>

<br/>
###API
None

###Javascript Code
After dragging the component into the design panel, in javascript editor panel, and it will generate the code ( `#componentId` is the component's id )： 

	$(document).on("gkComponentsReady", function () {
	  var dataset_tv = {
	    data: [
	      [1, 45],
	      [2, 44],
	      [3, 43],
	      [4, 42],
	      [5, 38]
	    ],
	    label: 'TV'
	  };
	
	  var dataset_online = {
	    data: [
	      [1, 25],
	      [2, 26],
	      [3, 26],
	      [4, 26],
	      [5, 20]
	    ],
	    label: 'Online'
	  };
	
	  var dataset_radio = {
	    data: [
	      [1, 17],
	      [2, 16],
	      [3, 15],
	      [4, 14],
	      [5, 12]
	    ],
	    label: 'Radio',
	    color: '#469a54'
	  };
	
	  var dataset_mobile = {
	    data: [
	      [1, 4],
	      [2, 6],
	      [3, 9],
	      [4, 12],
	      [5, 20]
	    ],
	    label: 'Mobile',
	    labels: ["4%", "6%", "9%", "12%", "20%"]
	  };
	
	  var options = {
	    xaxis: {
	      autoscaleMargin: 0.5,
	      ticks: [
	        [1, 2009],
	        [2, 2010],
	        [3, 2011],
	        [4, 2012],
	        [5, 2013]
	      ]
	    }
	  };
	
	  $('#componentId').gk('render', [dataset_tv, dataset_online, dataset_radio, dataset_mobile], options);
	});


<br/>
----------
Above is the description of `flot-line`. For more information, please back to [GK-Components-List](https://github.com/ezoapp/Learn-GK-Components).

Offical Site：[www.ezoui.com/app/](http://www.ezoui.com/app/)  
EZoApp Designer：[jqmdesigner.appspot.com/](http://jqmdesigner.appspot.com/)




