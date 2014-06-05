##Glinechart
`linechart` is a basic type of chart common in many fields. It is similar to a scatter plot except that the measurement points are ordered (typically by their x-axis value) and joined with straight line segments. Line Charts show how a particular data changes at equal intervals of time.

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
<td>width</td>
<td>Chart's width</td>
</tr>

<tr>
<td>height</td>
<td>Chart's height</td>
</tr>

<tr>
<td>cx</td>
<td>X-coordinate of the center of the chart</td>
</tr>

<tr>
<td>cy</td>
<td>Y-coordinate of the center of the chart</td>
</tr>

</table>

<br/>
###API
None

<br/>
###Javascript Code
After dragging the component into the design panel, in javascript editor panel, and it will generate the code ( `#componentId` is the component's id )：

	;
	$(document).one("pageshow", "#home", function aa() {
	  var chart = $("#componentId").gk("render", [0, 1, 2, 3, 4, 5], [
	    [1, 3, 5, 7, 9, 7],
	    [2, 5, 3, 1, 9, 12]
	  ], {
	    "colors": ["#f00", "#0000FF"],
	    nostroke: false,
	    "axis": "0 0 1 1",
	    "symbol": "circle",
	    smooth: true
	  });
	  chart.paper.label(25, 150, "Score").attr({
	    fill: "#fff",
	    stroke: "#000",
	    "stroke-width": 1
	  });
	}); 

<br/>
----------
Above is the description of `linechart`. For more information, please back to [GK-Components-List](https://github.com/ezoapp/Learn-GK-Components).

Offical Site：[www.ezoui.com/app/](http://www.ezoui.com/app/)  
EZoApp Designer：[jqmdesigner.appspot.com/](http://jqmdesigner.appspot.com/)




