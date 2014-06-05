##gk-device-motion
`flot-pie` is a circular chart divided into sectors, illustrating numerical proportion. 

<br/>
###Properties
Refer to flot's [pie chart](http://www.flotcharts.org/flot/examples/series-pie/index.html) Widget.

<br/>
###API
None


<br/>
###Javascript Code
After dragging the component into the design panel, in javascript editor panel, and it will generate the code ( `#componentId` is the component's id )：

	$(document).on("gkComponentsReady", function () {
	  var data = [{
	    label: 'Games',
	    data: 43
	  }, {
	    label: 'Social Networking',
	    data: 26
	  }, {
	    label: 'Entertainment',
	    data: 10
	  }, {
	    label: 'Utilities',
	    data: 10
	  }, {
	    label: 'News',
	    data: 2
	  }, {
	    label: 'Other',
	    data: 9
	  }];
	
	  $('#componentId').gk('render', data);
	});


<br/>
----------
Above is the description of `flot-pie`. For more information, please back to [GK-Components-List](https://github.com/ezoapp/Learn-GK-Components).

Offical Site：[www.ezoui.com/app/](http://www.ezoui.com/app/)  
EZoApp Designer：[jqmdesigner.appspot.com/](http://jqmdesigner.appspot.com/)




