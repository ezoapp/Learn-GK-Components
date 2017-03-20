## listview
`listview` Display data in list , you can switch page or do action on click item .  
listview contains two component：[`list-divider`](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-list-divider.md)  ( header ) 、[`listview-li`](https://github.com/ezoapp/Learn-GK-Components/blob/master/docs/GKComponent-listview-li.md) ( item ) 

### Properties
property			| setting
---						| ---
id						| component's id
style					| style attribute of the html element 
class					| class attribute of the html element
data-repeat   | set a **Truthy** value to enable rendering repetitive content by template. see the `model` api
Refer to JQueryMobile's [listview](http://api.jquerymobile.com/listview/) Widget.

### API

- **refresh()**：  
 	> Update and enhance the jQuery Mobile widgets within `listview`. <br/>
 	> If you update the content of `listview` via JavaScript, you must call the refresh method on it to update the visual styling. <br/>


- **autodividersSelector(selector)**:
  > Set the `autodividersSelector` function to `listview`'s option. <br/>


- **onRowEvent(event, handler(eventObject, data, index))**:
  > Attach an event handler function for one or more events to the **first-level non-list-divider** li of `listview`. <br/>
  > The handler function receives arguments: the event object passed by jQuery, the search index of the element in `listview`, and the data associated with the element (**if rendered by template with model data**). <br/>
  
  
- **onRow(handler)**：  
  > Attach a `click` event handler function for one or more events to the **first-level non-list-divider** li of `listview`. <br/>


- **onTapHold(handler)**:
  > Attach a `taphold` event handler function for one or more events to the **first-level non-list-divider** li of `listview`. <br/>


- **model(data)**：
  > If no arguments passed in, get the model data of `listvew`. <br/>
  > If `data` passed in, render the list items of `listview` by template. `data` can be a single JSON object or a JSON array. <br/>
  > The **template** is the html content within `<listview></listview>`, you can write `{{data-key}}` or `${data-key}` to represent that you want the template to replace those patterns with corresponding value of the model data. <br/> 
  > For example:
    ```html
      <ul data-role="listview" is="listview" data-repeat="true">
        <li data-role="list-divider">{{userId}}</li>
        <li is="listview-li">{{userName}}</li>
      </ul>    
    ```
    After passing the model data, `listview` will repetitively render the list items by template and replace the `{{userId}}` and `{{userName}}` with the JSON object's corresponding value. <br/>
    Notice that you have to set the `data-repeat` attribute as **Truthy** to enable template rendering in advance. If the `data-repeat` is a `string` value, `listview` will try to check if the same named property of `data` is an array then use as the model data. <br/>

   
- **addRow(data)**:
  > Append a list item to the end of `listvew` and the item is rendered by the template with given data. <br/>
  > Notice that you have to set the `data-repeat` attribute as **Truthy** to enable template rendering in advance. <br/>


- **insertRow(data, index)**:
  > Insert a list item to the specific index of `listvew` and the item is rendered by the template with given data. <br/>
  > Notice that you have to set the `data-repeat` attribute as **Truthy** to enable template rendering in advance. <br/>
  

- **removeRow(index)**:
  > Remove the list item from `listview` according to the given index.


----------
Above is the description of `listview`. For more information, please back to [GK-Components-List](https://github.com/ezoapp/Learn-GK-Components).

EZoApp Official Site: [ezoui.com](http://ezoui.com/)  





