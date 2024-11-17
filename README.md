# EMSC Near Real Time Earthquake Notifications

## Home Assistant Custom Component for Near Realtime Notifications of Earthquakes from EMSC


EMSC Provides Earthquake Information from https://seismicportal.eu/realtime.html websocket connection instantly. This custom component provides websocket connection to EMSC servers and gets the information to Home Assistant instantly. 

<p align="center">
<img src="images/Screenshot 2024-11-17 at 12.50.37.png" width="400" height="400">
</p>

## Installation

You will need to install the crowipmodule manually.

- Create custom_components folder if it does not exist to get following structure `config/custom_components`

- Create crowipmodule folder inside custom_components folder `config/custom_components/crowipmodule`

- Copy all files from [custom_components/emsc_earthquake/](custom_components/emsc_earthquake/) into the previously created folder

- Restart Home Assistant

## Setup and Configuration

- Go to `Settings/Devices & services`

- Press `+Add Integration` button

- Select `EMSC Earthquake`

<p align="left">
<img src="images/Screenshot 2024-11-17 at 12.33.17.png" width="400" height="600">
</p>

- __name :__ Name of the sensor

- __center_latitude:__ Latitude of your base location, default is zone.home latitude

- __center_logitude:__ Longitude of your base location, default is zone.home longitude

- __radius_km:__ Distance of all earthquakes to be informed of, within a radius from your base location (in km)

- __min_mag:__ Minimum magnitude of earthquakes to be informed of, within the radius defined earlier.

- __total_max_mag:__ Independent from earlier parameters, show all earthquakes larger than this magnitude from all over the world.

  
