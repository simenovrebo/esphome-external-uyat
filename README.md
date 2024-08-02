## uyat
This is a copy of the esphome's Tuya component with some of my modifications that were not (yet?) accepted to the mainline of esphome.
Namely:
- Setup priority adjusted to initialize TuyaMCU without waiting for wifi connection
- Fix for a Tuya Number to be able to work with enums
...

## Usage
You can use it exactly the same as you would use the origina Tuya component, except you specify "uyat" instead of "tuya", eg:
```yaml
uyat:

...

switch:
  - platform: "uyat"
    switch_datapoint: 1
    name: "On/Off Switch"

```