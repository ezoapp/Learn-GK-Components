##controlgroup-radio
To create a set of radio buttons, add an input with a `type="radio`" attribute and a corresponding label. Set the for attribute of the label to match the id of the input so they are semantically associated.

The label element is displayed next to the radio form element. Wrap the radio buttons in a fieldset element that has a legend which acts as the title for the question.

To visually integrate multiple radio buttons into a vertically grouped button set, the framework will automatically remove all margins between buttons and round only the top and bottom corners of the set if there is a `data-role="controlgroup"` attribute on the container

<br/>
###Properties
Refer to JQueryMobile's [controlgroup-radio](http://api.jquerymobile.com/checkboxradio/) Widget.

<br/>
###API

- **model**：  
  	> description。

			$('#test').gk().model();

- **apply**：  
  	> description。

			$('#test').gk().apply();

- **checked**：  
  	> description。

			$('#test').gk().checked();

- **unchecked**：  
  	> description。

			$('#test').gk().unchecked();

- **onSelect**：  
  	> description。

			$('#test').gk().onSelect();

- **disable**：  
  	> description。

			$('#test').gk().disable();

- **enable**：  
  	> description。

			$('#test').gk().enable();
<br/>
----------
Above is the description of `controlgroup-radio`. For more information, please back to [GK-Components-List](https://github.com/ezoapp/Learn-GK-Components).

Offical Site：[www.ezoui.com/app/](http://www.ezoui.com/app/)  
EZoApp Designer：[jqmdesigner.appspot.com/](http://jqmdesigner.appspot.com/)




