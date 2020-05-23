# frost_risks
Frost risks sensors for HA (absolute humidity, dew point, freezing point and frost risk levels)

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

#### Required
- temperature_sensor
- humidity_sensor

#### Optional
- friendly_name
- icon_template
- entity_picture_template

## Screenshots

#### Absolute Humidity


#### Dew Point


#### freezing Point


#### Risk level



