

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
# frost_risks
Frost risks sensors for HA (absolute humidity, dew point, freezing point and frost risk levels)

Based on / ripped off from : https://github.com/papo-o/home-assistant-frost-risks

I would have used @papo-o's version , but it just didn't load in HA and it had a logic check missing

[@papo-o]( https://github.com/papo-o

## Installation

Use [hacs](https://custom-components.github.io/hacs/) with this repo URL https://github.com/redlegoman/home-assistant-frost-risks or copy `custom_components/` to your HA configuration.

## Usage

To use, add the following to your `configuration.yaml` file:

```
sensor:
  - platform: frost_risks
    sensors:
      livingroom:
        friendly_name: Living Room
        temperature_sensor: sensor.temperature_livingroom
        humidity_sensor: sensor.humidity_livingroom
      bedroom:
        ...

```
also you can add dark Sky apparent temperature and humidity 12 hours sensors for predict a risk

```
      frost_prevision:
        friendly_name: prevision à 12 h
        temperature_sensor: sensor.dark_sky_apparent_temperature_12h
        humidity_sensor: sensor.dark_sky_humidity_12h
```


#### Required
- temperature_sensor
- humidity_sensor

#### Optional
- friendly_name
- icon_template
- entity_picture_template

