## json-selectmenu
`json-selectmenu` can render a select-menu widget by loading json data from backend service.

<br/>
### Properties
- **service**：  
Define the JSON Data web service url. [http://ezodemo.github.io/data/vacationTypes.json](http://ezodemo.github.io/data/vacationTypes.json) is a simple example.

For any other properties, please refer to JQueryMobile's [selectmenu](http://api.jquerymobile.com/selectmenu/) Widget.

<br/>
### API

- **refresh**：  
  > If you set data to selectmenu via JavaScript , you must call the refresh method on it to update the visual styling.

    $('#selectmenu').gk().refresh();

- **model**：  
    > Set data to selectmenu , data type is JSON Array.

      var data = [
        {
            "text":"Annual Leave",
            "value":"V"
            },
            {
            "text":"Sick Leave",
            "value":"D"
            },
            {
            "text":"General Leave",
            "value":"E"
            },
            {"text":"Wedding Leave",
             "value":"W"
            }
        ];
        $('#selectmenu').gk().model(data);

    > HTML template pattern {{data.key}}

      <select id="gk-57grpH" is="json-selectmenu" service="http://ezodemo.github.io/data/vacationTypes.json">
          <option value="{{value}}">{{text}}</option>
        </select>             

- **value**：  
    > Assign a default value to the select-menu.
```javascript 
    $('#selectmenu').gk().value("E");
```

- **enable**：  
    > such as the `enable` method of jquery-mobile. See http://api.jquerymobile.com/selectmenu/#method-enable 

- **disable**：  
    > such as the `disable` method of jquery-mobile. See http://api.jquerymobile.com/selectmenu/#method-disable

- **open**：  
    > such as the `open` method of jquery-mobile. See http://api.jquerymobile.com/selectmenu/#method-open

- **close**：  
    > such as the `close` method of jquery-mobile. See http://api.jquerymobile.com/selectmenu/#method-close

- **open**：  
    > such as the `open` method of jquery-mobile. See http://api.jquerymobile.com/selectmenu/#method-open



<br/>
### Javascript Code
Unlike most of our widgets generating tone of javascript code, this widget generates no code but html. All the javascript logic executes inside the component itself. This means you've no need to maintain those generated code any more, leave the code more clean and easy to maintain. 

<br/>
----------
Above is the description of `json-selectmenu`. For more information, please back to [GK-Components-List](https://github.com/ezoapp/Learn-GK-Components).

EZoApp Official Site: [ezoui.com](http://ezoui.com/)





