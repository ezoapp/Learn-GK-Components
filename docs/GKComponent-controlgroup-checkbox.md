##controlgroup-checkbox
Typically, there are multiple checkboxes listed under a question title. To visually integrate multiple checkboxes into a grouped button set, the framework will automatically remove all margins between buttons and round only the top and bottom corners of the set if there is a `data-role="controlgroup"` attribute on the fieldset. 

<br/>
###Properties
Refer to JQueryMobile's [checkbox-button](http://api.jquerymobile.com/checkboxradio/) Widget.

<br/>
###API

- **model**：  
  	> Set data to controlgroup-checkbox , data type is JSON Array.
            
        var data = [{
          item: 'Swimming'
        }, {
          item: 'Shopping'
        }, {
          item: 'Singing'
        }];

        $('#c1').gk().model(data);
          
  	> HTML template pattern {{data.key}}
  	
        <fieldset data-role="controlgroup" data-type="vertical" is="controlgroup-checkbox" id="c1">
          <legend>Interest</legend>
          <input type="checkbox" value="{{item}}">
          <label>${item}</label>
        </fieldset>

- **apply**：  
  	> Set data to controlgroup-checkbox when data is only one , data type is JSON object

        var data = {
            item1: 'Swimming',
            item2: 'Shopping',
            item3: 'Singing'
        }

        $('#c1').gk().apply(data);

  	> HTML template pattern {{data.key}}
  	
        <fieldset data-role="controlgroup" data-type="vertical" is="controlgroup-checkbox" id="c1">
          <legend>Interest</legend>
          <input type="checkbox" value="{{item1}}">
          <label>${item1}</label>
          <input type="checkbox" value="{{item2}}">
          <label>${item2}</label>
          <input type="checkbox" value="{{item3}}">
          <label>${item3}</label>
        </fieldset>


- **onSelect(callback))**：  
  	> When you click on checkbox item , onSelect will be invoke.  
    > If set data by model API , first argument of callback is JSON object.  
    > If set data by apply API , first argument of callback is input element of JQuery.

          // If call model API , callback argument is value object
          $('#controlgroup-checkbox').gk().model(data);
          $('#controlgroup-checkbox').gk().onSelect(function(vo) {

          });

          // If call apply API , callback argument is input element of JQuery
          $('#controlgroup-checkbox').gk().apply(data);
          $('#controlgroup-checkbox').gk().onSelect(function($input) {

          });    


- **disable(rowNum)**：  
  	> Disable the item.  
    > rowNum starting from 0.  
    > Disable all when rowNum is null. 

        $('#controlgroup-checkbox').gk().disable();


- **enable(rowNum)**：  
  	> Enable the item.  
    > rowNum starting from 0.  
    > Enable all when rowNum is null. 

        $('#controlgroup-checkbox').gk().enable();
			


- **checked(rowNum)**：  
  	> Select the item.
    > rowNum starting from 0.  
    > Return input value. 

        $('#controlgroup-checkbox').gk().checked(0);



- **unchecked(rowNum)**：  
  	> Unselect the item.  
    > rowNum starting from 0.  
    > Return input value. 

        $('#controlgroup-checkbox').gk().unchecked(0);




<br/>
----------
Above is the description of `controlgroup-checkbox`. For more information, please back to [GK-Components-List](https://github.com/ezoapp/Learn-GK-Components).

Offical Site：[www.ezoui.com/app/](http://www.ezoui.com/app/)  
EZoApp Designer：[jqmdesigner.appspot.com/](http://jqmdesigner.appspot.com/)




