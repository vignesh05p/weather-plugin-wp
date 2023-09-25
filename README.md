# weather-plugin-wp
Plugin should be able to display the weather of the current location or weather of Delhi.
A weather widget for WordPress featuring data provided by the OpenWeatherMap.org API. See (https://openweathermap.org) for details.

Description
The plugin parses data returned by the OpenWeatherMap.org API to display weather information of a given location. All weather data is cached at least for three hours, unless you use the geolocation feature (not cached). Use as a widget or add a shortcode like this (e.g. in posts, ...):

[weather location="London, UK" units="imperial" override_title="Weather" forecast_days="0" show_stats="false"]

You can also use the city ID instead of the name. This is the recommended way to do it, because it's much more precise than the name:

[weather location="2657896" units="metric" forecast_days="3" show_stats="0"]

The provided API key is connected to a free account for demo purposes only. In order to not get banned due to heavy usage, you should use your own API key instead; either in the widget configuration or by using the shortcode:

[weather location="2657896" openweathermap_api_key="<insert your API key here>"]

Please note that I do not provide an empty index.php file with my WordPress plugins, because security by obscurity is poor man's choice instead of using a proper configuration.

Settings
Location: Enter something like Long Beach, CA or just Los Angeles. Alternatively enter the location ID as provided on the OpenWeatherMap.org website. To use the browser's geolocation capabilities enable the "automatic" option. This will disable the location input field.
Units: °F or °C (default).
Forecast: Shows forecast weather information for the configured number of days.
Override location title: Change the title of the location.
OpenWeatherMap API key: Provide your own API key here to circumvent limitations of my free account.
Show details: Show things like humidity, wind, highs and lows etc.
Link to extended forecast: Make the location clickable. Opens details page of the configured location in a new tab when clicked.
Installation
Add plugin to the plugins folder.
Activate the plugin.
Use a shortcode or the widget.
Privacy policy
This widget itself does not collect, store or analyze any personal data. However, by using the OpenWeatherMap.org API such data may be transferred to or requested by OpenWeatherMap.org in order to provide you weather information of the location information you provided. For details please see their privacy policy at https://openweathermap.org/privacy-policy
