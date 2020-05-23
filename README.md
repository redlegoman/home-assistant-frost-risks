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

![absolute_humidity](https://user-images.githubusercontent.com/25136535/82730932-c8f23280-9d03-11ea-8c4b-a84d112f1a49.png)

#### Dew Point

![dewpoint](https://user-images.githubusercontent.com/25136535/82730959-ee7f3c00-9d03-11ea-8fad-86e08c5b52ae.png)

#### freezing Point

![freezing_point](https://user-images.githubusercontent.com/25136535/82730895-7fa1e300-9d03-11ea-9329-8109b1a5c4f6.png)

#### Risk level



