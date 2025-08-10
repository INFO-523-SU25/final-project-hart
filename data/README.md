# Data
-   **[mn_weather_data]**:
  
-   **[storm_data_search_results]**: Historical tornado data dating back to the 1950's from the US NOAA. The data contains all of the data for every reported tornado in the state of Minnesota. For the purposes of this analysis the data will only be used corresponding to available daily data 2020-2025. If more data is needed I will update this!

# Codebook for [mn_weather_data] Dataset

|        Variable Names       |       Data Types      | Description | Unit |
|-----------------------------|-----------------------|-------------|------|
| date	                      | TimeDate | Data and Time of weather collection | (YYYY-MM-DD hh-mm-ss) |
| weather_code                | Float    | The most severe weather condition on a given day | (WMO Code) |
| temperature_2m_mean         | Float    | Mean daily air temperature at 2 meters above ground | (°F) |
| temperature_2m_max          | Float    | Maximum daily air temperature at 2 meters above ground | (°F) |
| temperature_2m_min          | Float    | Minimum daily air temperature at 2 meters above ground | (°F) |
| precipitation_sum           | Float    | Sum of daily precipitation (including rain, showers and snowfall) | (mm) |
| rain_sum                    | Float    | Sum of daily rain | (mm) |
| snowfall_sum                | Float    | Sum of daily snowfall | (cm) |
| wind_speed_10m_max          | Float    | Maximum wind speed on a day | (mph) | 
| wind_gusts_10m_max	        | Float    | Maximum wind gusts on a day | (mph) |
| wind_direction_10m_dominant	| Float    | Dominant wind direction | (°) |
| dew_point_2m_mean	          | Float    | Mean daily dew point at 2 meters above ground | () |
| dew_point_2m_max	          | Float    | Maximum daily dew point at 2 meters above ground | () |
| dew_point_2m_min	          | Float    | Minimum daily dew point at 2 meters above ground | () |
| relative_humidity_2m_mean	  | Float    | Mean daily relative humidiity at 2 meters above ground | () |
| relative_humidity_2m_max	  | Float    | Maximum daily relative humidity at 2 meters above ground | () |
| relative_humidity_2m_min    | Float    | Minimum daily relative humidity at 2 meters above ground | () |
| surface_pressure_mean	      | Float    | Mean daily pressure at surface | () |
| surface_pressure_max	      | Float    | Maximum daily pressure at surface | () |
| surface_pressure_min        | Float    | Minimum daily daily pressure at surface | () |

# Codebook for [storm_data_search_results] Dataset

|        Variable Names       |       Data Types      | Description | 
|-----------------------------|-----------------------|-------------|

