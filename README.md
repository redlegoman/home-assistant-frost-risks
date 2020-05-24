[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
# frost_risks
Frost risks sensors for HA (absolute humidity, dew point, freezing point and frost risk levels)

## Installation

Use [hacs](https://custom-components.github.io/hacs/) with this repo URL https://github.com/papo-o/home-assistant-frost-risks or copy `custom_components/` to your HA configuration.

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


## Todo List

- notification examples

## Screenshots

#### Absolute Humidity

![absolute_humidity](https://user-images.githubusercontent.com/25136535/82730932-c8f23280-9d03-11ea-8c4b-a84d112f1a49.png)

#### Dew Point

![dewpoint](https://user-images.githubusercontent.com/25136535/82730959-ee7f3c00-9d03-11ea-8fad-86e08c5b52ae.png)

#### freezing Point

![freezing_point](https://user-images.githubusercontent.com/25136535/82730895-7fa1e300-9d03-11ea-9329-8109b1a5c4f6.png)

#### Risk level

![riskLevel](https://user-images.githubusercontent.com/25136535/82762799-6aac7900-9e03-11ea-9611-27ed1757561b.png)

### With Dark Sky sensors for 12 hours prediction 

![darkskyPredic](https://user-images.githubusercontent.com/25136535/82763079-2ae69100-9e05-11ea-8af8-5c26363e5a83.png)

