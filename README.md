# EMSC Near Real Time Earthquake Notifications

## Home Assistant Custom Component for Near Realtime Notifications of Earthquakes from EMSC


EMSC Provides Earthquake Information from https://seismicportal.eu/realtime.html websocket connection instantly. This custom component provides websocket connection to EMSC servers and gets the information to Home Assistant instantly. 

<p align="center">
<img src="images/Screenshot 2024-11-17 at 12.50.37.png" width="400" height="400">
</p>

## Installation (manual)

You can install the emsc_earthquake manually.

- Create custom_components folder if it does not exist to get following structure `config/custom_components`

- Create emsc_earthquake folder inside custom_components folder `config/custom_components/emsc_earthquake`

- Copy all files from [custom_components/emsc_earthquake/](custom_components/emsc_earthquake/) into the previously created folder

- Restart Home Assistant

## Installation via HACS (Add a Custom Repository)

1. Open **Home Assistant**.
2. Navigate to **HACS** in your sidebar.
3. Click the **three dots `⋮`** in the top right corner and select **Custom repositories**.
4. Paste the URL of this repository into the **Repository** field: `https://github.com/febalci/ha_emsc_earthquake`
5. Select **Integration** as the category.
6. Click **Add** and wait for it to appear in the list.
7. Now search for **EMSC Earthquake** in HACS and download it.
8. Restart Home Assistant to finalize the installation.

## Setup and Configuration

- Go to `Settings/Devices & services`

- Press `+Add Integration` button

- Select `EMSC Earthquake`

<p align="left">
<img src="images/Screenshot 2024-11-17 at 12.33.17.png" width="400" height="600">
</p>

- __name :__ Name of the sensor

- __center_latitude:__ Latitude of your base location, default is zone.home latitude

- __center_longitude:__ Longitude of your base location, default is zone.home longitude

- __radius_km:__ Distance of all earthquakes to be informed of, within a radius from your base location (in km)

- __min_mag:__ Minimum magnitude of earthquakes to be informed of, within the radius defined earlier.

- __total_max_mag:__ Independent from earlier parameters, show all earthquakes larger than this magnitude from all over the world.

  
