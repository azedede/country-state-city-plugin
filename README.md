## Welcome to Jquery Country-State-City-Plugin

THis plugin solve problem of country state city dropdown with simple implementation.

You can use this plugin in any application.

### Implementation Step

1) copy below script at the bottom of you body tag

<script src="https://code.jquery.com/jquery-3.3.1.min.js"></script>  
<script type="text/javascript" src="countrystatecity.min.js"></script> 
  
  ## Important Notes:- You must specify the "element-id" attribute to each select option and each select element has class "countrystatecity"
        for country element-id = "country"
            state element-id = "state"
            city element-id = "city"
        define class="countrystatecity" for each element
        ### each element should have one unique id. id should be any thing but unique. 
	example:- 
	<select name="p_country" element-id="country" dependent-state-id="state_id1" dependent-city-id="city_id1" id="country_id1"  class="countrystatecity">
					<option value="">select country</option>
	</select><select name="p_state" element-id="state" dependent-city-id="city_id1" id="state_id1" id="state_id1" class="countrystatecity"><option value="">select</option></select> <select name="p_city" element-id="city" id="city_id1" class="countrystatecity"><option value="">select</option></select>
	#### Note:- dependent-state-id should be unique id of state select drop down and same is apply on dependent-city-id  

Now you have to write this code at bottom of body tag inside script

	$(document).ready(function(){
		$('.countrystatecity').countrystatecity();
	});
```

### For prefilled dropdown you have to changes a little bit
1) in country select dropdown 
	# selected-value="101"
2) in state select dropdown 
	# selected-value="5"
3) in city select dropdown
	# selected-value="459"
	## Note:- selected-value should be the value of state, country, or city. what ever you want

### Thank You, Done.
for demo https://absharalam.github.io/country-state-city-plugin/
