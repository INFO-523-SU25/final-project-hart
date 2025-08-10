# Data
-   **[mn_weather_data]**: Daily weather data coming out of the Mineapolis Saint Paul (Twin Cities) Weather Center at MSP international airport. The data has been synthesized from the open-meteo API for all days from Jan 1 2020 to December 31 2024. It contains most weather stats plus some advanced stats pertaining to wind speeds, CAPE, etc. 
  
-   **[storm_data_search_results]**: Historical tornado data dating back to the 1950's from the US NOAA. The data contains all of the data for every reported tornado in the state of Minnesota. For the purposes of this analysis the data will only be used corresponding to available daily data 2020-2025. If more data is needed I will update this!

# Codebook for [mn_weather_data] Dataset

|        Variable Names       |Data Types| Description | Unit |
|-----------------------------|----------|-------------|------|
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

|    Variable Names   |       Data Types      | Description |  Unit |
|---------------------|-----------------------|-------------|-------|
| EVENT_ID            | Int | ID assigned by NWS to note a single, small part that goes into a specific storm episode | Database ID |
| CZ_NAME_STR         | String | County/Parish, Zone or Marine Name assigned to the county FIPS number or NWS Forecast Zone | None |
| BEGIN_LOCATION      | String | 
| BEGIN_DATE          | Date | 
| BEGIN_TIME          | Time | 
| EVENT_TYPE          | String | Type of Storm Event (ex. Tornadoes, Hail, etc.) | None | 
| MAGNITUDE           | 
| TOR_F_SCALE         | String | Enhanced Fujita Scale describes the strength of the tornado based on the amount and type of damage caused by the tornado | Fujita Scale |
| DEATHS_DIRECT       |
| INJURIES_DIRECT     |
| DAMAGE_PROPERTY_NUM | 
| DAMAGE_CROPS_NUM    |
| STATE_ABBR          |
| CZ_TIMEZONE         |
| MAGNITUDE_TYPE      |
| EPISODE_ID          |
| CZ_TYPE             | String | Type of Jurisdiction (County/Parish, Zone or Marine Name) | None |
| CZ_FIPS             | Int | FIPS ID number given to County/Parish, Zone or Marine Name | FIPS Code | 
| WFO                 |
| INJURIES_INDIRECT   |
| DEATHS_INDIRECT     |
| SOURCE              |
| FLOOD_CAUSE         |
| TOR_LENGTH          | Float | Length of the tornado or tornado segment while on the ground | (Miles) |
| TOR_WIDTH           | Int | Width of the tornado or tornado segment while on the ground | (Yards) |
| BEGIN_RANGE         |
| BEGIN_AZIMUTH       |
| END_RANGE           |
| END_AZIMUTH         |
| END_LOCATION        |
| END_DATE            |
| END_TIME            |
| BEGIN_LAT           | Float | The latitude where the event began | (°) |
| BEGIN_LON           | Float | The longitude where the event began | (°) |
| END_LAT             | Float | The latitude where the event ended | (°) |
| END_LON             | Float | The longitude where the event ended | (°) |
| EPISODE_NARRATIVE   | Sentence | The episode narrative depicting the general nature and overall activity of the episode. The narrative is created by NWS. | None | 
| EVENT_NARRATIVE     | Sentence | The event narrative provides more specific details of the individual event. The event narrative is provided by NWS. | None |
