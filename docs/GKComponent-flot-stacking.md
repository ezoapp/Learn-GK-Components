##flot-stacking
`flot-stacking` is used when data sets have to be broken down into their constituents, and then the data sets as a whole also need to be compared against one another.

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
None


<br/>
###Javascript Code
After dragging the component into the design panel, in javascript editor panel, and it will generate the code ( `#componentId` is the component's id )：

	  $(document).on("gkComponentsReady", function () {
	    var data = [{
	      label: 'Apps',
	      data: [
	        [0, 80],
	        [1, 86],
	      ],
	      color: '#50b4f6'
	    }, {
	      label: 'Mobile Web',
	      data: [
	        [0, 20],
	        [1, 14],
	      ],
	      color: '#9e9e9e'
	    }];
	
	    var options = {
	      yaxis: {
	        autoscaleMargin: 0.2,
	      }
	    };
	
	    $('#componentId').gk('render', data, options);
	  });

<br/>
----------
Above is the description of `flot-stacking`. For more information, please back to [GK-Components-List](https://github.com/ezoapp/Learn-GK-Components).

EZoApp Official Site: [ezoui.com](http://ezoui.com/)




