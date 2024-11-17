# EMSC Near Real Time Earthquake Notifications

## Home Assistant Custom Component for Near Realtime Notifications of Earthquakes from EMSC


EMSC Provides Earthquake Information from https://seismicportal.eu/realtime.html websocket connection instantly. This custom component provides websocket connection to EMSC servers and gets the information to Home Assistant instantly. 

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

- 
