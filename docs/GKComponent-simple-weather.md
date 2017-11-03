## simple-weather
`simple-weather`

### Properties
<table>

<tr>
    <th>property</th>
    <th>setting</th>
</tr>

<tr>
    <td>id</td>
    <td>Component's id</td>
</tr>

<tr>
    <td>style</td>
    <td>HTML inline style</td>
</tr>

<tr>
    <td>geolocation</td>
    <td>Get current geolocation or not, default false</td>
</tr>

<tr>
    <td>location</td>
    <td>Location's weather, like Taipei, Kaohsiung, etc...</td>
</tr>

<tr>
    <td>unit</td>
    <td>Temperature unit, c or f</td>
</tr>

<tr>
    <td>autoupdate</td>
    <td>Auto update frequency, millisecond</td>
</tr>

</table>

### API

- **geolocation**：
  > Get or set current geolocation
  ```javascript
    // Get
    var isGetCurrentGeolocation = $('#weather').gk().geolocation();

    // Set
    $('#weather').gk().geolocation(true);
  ```

- **location**：
  > Get or set location
  ```javascript
    // Get
    var location = $('#weather').gk().location();

    // Set
    $('#weather').gk().location('Kaohsiung');
  ```

- **unit**：
  > Get or set unit
  ```javascript
    // Get
    var unit = $('#weather').gk().unit();

    // Set
    $('#weather').gk().unit('f');
  ```

- **autoupdate**：
  > Set auto update frequency, 0 = stop
  ```javascript
    $('#weather').gk().autoupdate(10000);
  ```

- **refresh**：
  > Refresh immediately
  ```javascript
    $('#weather').gk().refresh();

    // Catch failure
    $('#weather').gk().refresh(function() {
        console.log('fail');
    });
  ```

----------
Above is the description of `simple-weather`. For more information, please back to [GK-Components-List](https://github.com/ezoapp/Learn-GK-Components).

EZoApp Official Site: [ezoui.com](https://ezoui.com/)
