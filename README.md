# rejoice-weather

simple ESP8266 weather station

## Develop

You'll want to clone this repository, create a python3 virtual enviroment, install [esphome](https://esphome.io/guides/getting_started_command_line.html), and do a first compile to install dependencies:

```
git clone git@github.com:jameshome/rejoice-weather.git
cd rejoice-weather
python3 -m venv $PWD
source $PWD/bin/activate.fish
pip3 install esphome
esphome rejoice_weather.yaml compile
```

You'll want to create a
[secrets.yaml](https://www.home-assistant.io/docs/configuration/secrets/) — search the codebase for `!secret` to see what it should specify.

If your compile is successful, it's time to connect your board and upload your configuration to it:

```
esphome rejoice_weather.yaml run
```
