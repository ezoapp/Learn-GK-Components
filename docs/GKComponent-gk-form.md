## gk-form
`gk-form` provide users to get and set value to components inside, and basic validation.

### Current support components
The following components will auto refresh and enhance when setting data.

* text-input
* range-input
* search-input
* controlgroup-radio
* controlgroup-checkbox
* flipswitch
* textarea-input

### Properties
The same with the normal html form element.

### API

- **info([data])**：  
  > Sending data to set values to components, or get values from components inside.  The key is component's name or id (default).

      var data = {
        'f1': 'test1',
        'f2': 'test2'
      };
      $('#form1').gk().info(data);

      var info = $('#form1').gk().info();

 ``` html
  <form id='form1' is='gk-form'>
    <input type='text' name='f1' required>
    <textarea name="f2" required></textarea>
  </form>
 ```

- **valid**：  
  > Check if the form is valid and show the error messages.

      // return true or false
      $('#form1').gk().valid();

----------
Above is the description of `gk-form`. For more information, please back to [GK-Components-List](https://github.com/ezoapp/Learn-GK-Components).

EZoApp Official Site: [ezoui.com](https://ezoui.com/)





