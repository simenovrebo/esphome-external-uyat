## uyat
This is a copy of the esphome's Tuya component with some of my modifications that were not (yet?) accepted to the mainline of esphome.
Namely:
- Setup priority adjusted to initialize TuyaMCU without waiting for wifi connection [this PR]([esphome/esphome#7028](https://github.com/esphome/esphome/pull/7028))
- ...
  (the rest of changes have already been integrated in esphome)


## Usage
You can use it exactly the same as you would use the original Tuya component, except you specify "uyat" instead of "tuya", eg:
```yaml
uyat:

...

switch:
  - platform: "uyat"
    switch_datapoint: 1
    name: "On/Off Switch"

```
