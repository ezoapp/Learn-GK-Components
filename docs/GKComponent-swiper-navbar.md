## swiper-navbar
`swiper-navbar` provide the feature to swipe navagation bar if having too many content on it.

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
<td>data-slides-per-view</td>
<td>Default number of slides to show in one page</td>
</tr>

<tr>
<td>data-display-name</td>
<td>Default display name when slides generated dynamically</td>
</tr>

</table>

### API

- **swiper**：  
  > Original swiper object.
  > Use this swiper object to get more function.

        var swiper = $('#swiper').gk().swiper(),
          index = swiper.clickedIndex,
          slide = swiper.clickedSlide;

- **onSlideClick(callback)**：  
 > Trigger callback function when clicking each slide.

		  $('#swiper').gk().onSlideClick(function(swiper, event, data, index) {
            var slide = swiper.clickedSlide;
          });

- **appendSlide(data[, removeAll])**：  
  > Dynamically append slides from data.  
  > Set removeAll to true to clean all slides first. 

		$('#swiper').gk().appendSlide(["One", "Two", "Three"]);
        $('#swiper').gk().appendSlide([{name:"One"}, {name:"Two"}, {name:"Three"}], true);

- **slideTo(index)**：  
  > Swipe slide. 

		$('#swiper').gk().slideTo(0);


----------
Above is the description of `swiper-navbar`. For more information, please back to [GK-Components-List](https://github.com/ezoapp/Learn-GK-Components).

EZoApp Official Site: [ezoui.com](https://ezoui.com/)
