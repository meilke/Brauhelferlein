# Brauhelferlein

Automatisierung des Maische Kochens mit minimalem Aufwand und lediglich eines ESP 8266 eigenständig für keine 10€.

## Highlights

- Temperatur PID Regelung auf zehntel Grad genau
- Rührwerk Drehzahlregelung
- Rührwerk Interwall Steuerung
- Graphen für Temperatur Verlauf
- Rast Zeit Erkennung
- Verwendet Wifi Zugang oder stellt eigenen AP bereit
- Web Flash Update

### Screenshot

![Screenshot](docs/screenshot.png)

## Anleitung

### Benötigt wird

- ein ESP8266 (D1 mini oder ESP-12E)
- ein Relais oder SSR
- ein DS18B20 Messfühler
- zur Steuerung des Maische Rührwerks (Scheibenwischermotor) einen Motortreiber, z.B. VNH2SP30
- optional ein Display (LCD I2C 1602).

### Verkabelung
<img src="https://rawgit.com/universam1/Brauhelferlein/master/docs/Wiring.svg" width="100%" height="300">

### Software

- Arduino 1.6.x
- erweitern mit [ESP8266 Arduino](https://github.com/esp8266/Arduino)
- Installiere libraries
  - OneWire.h
  - DallasTemperature.h
  - NewLiquidCrystal: https://bitbucket.org/fmalpartida/new-liquidcrystal/wiki/Home (bitte [1.2.1](https://bitbucket.org/fmalpartida/new-liquidcrystal/downloads/) benutzen)
  - PID_v1.h
  - ArduinoJson.h
  - ESPAsyncTCP: https://github.com/me-no-dev/ESPAsyncTCP
  - ESPAsyncWebServer: https://github.com/me-no-dev/ESPAsyncWebServer

### BOM for project including case

[Case](docs/BOM-Case.md)

Enjoy your beer! :)
