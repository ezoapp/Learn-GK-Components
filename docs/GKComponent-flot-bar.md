## flot-bar
`flot-bar` is a chart with rectangular bars with lengths proportional to the values that they represent. The bars can be plotted vertically or horizontally. A vertical bar chart is sometimes called a column bar chart. 

### Properties
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

### API
None


### Javascript Code
After dragging the component into the design panel, in javascript editor panel, and it will generate the code ( `#componentId` is the component's id )：

	$(document).on("gkComponentsReady", function () {
	  var data = [{
	    label: 'Games',
	    data: [
	      ['Games', 32]
	    ]
	  }, {
	    label: 'Facebook',
	    data: [
	      ['Facebook', 17]
	    ]
	  }, {
	    label: 'Browser',
	    data: [
	      ['Browser', 14]
	    ]
	  }, {
	    label: 'Social Messaging',
	    data: [
	      ['Social Messaging', 9.5]
	    ]
	  }, {
	    label: 'YouTube',
	    data: [
	      ['YouTube', 4]
	    ]
	  }, {
	    label: 'Entertainment',
	    data: [
	      ['Entertainment', 4]
	    ]
	  }, {
	    label: 'Utilities',
	    data: [
	      ['Utilities', 8]
	    ]
	  }, {
	    label: 'News',
	    data: [
	      ['News', 3]
	    ]
	  }, {
	    label: 'Other',
	    data: [
	      ['Other', 8.5]
	    ]
	  }];
	
	  $('#componentId').gk('render', data);
	});

----------
Above is the description of `flot-bar`. For more information, please back to [GK-Components-List](https://github.com/ezoapp/Learn-GK-Components).

EZoApp Official Site: [ezoui.com](http://ezoui.com/)




