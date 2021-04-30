# TWIR - The worst Internet radio

## Requirements

### Functional
* Be an Internet radio, duh
* Powered from USB-C port
* Can be also powered from rechargeable (through USB port) batteries
* Have the function to be a Bluetooth speaker
* Stereo speakers
* Small display indicating station, mode, volume, battery charge, weather today etc etc
* Mayyyybeeeee speech commands, just maybe

### Non-functional
* Software mp3 decoding
* Optional other codecs support

### Requirements for usage
* Day of working on battery power supply
* Clear indication (through leds or display) of current mode: radio/Bluetooth speaker
* Clear indication of charge levels
* Have nice dial for choosing options

## Planned setup
* ESP32 - for Wi-Fi & Bluetooth connectivity
* STM32 with FPU and DSP extensions (STM32F4/STM32F7?) - for signal (audio) processing? That could be ESP32 too
* I2S DAC - for dat sound quality, e.g. UDA1334A [example](https://botland.com.pl/odtwarzacze-mp3-wav-ogg-midi/10871-uda1334a-i2s-dekoder-stereo-dac-adafruit-3678.html)
* Energy efficient audio amplifier if not present in above
* Some kind of USB-C IC
* Some kind of speakers

1st version:

Input - 5V USB-C __without__ USB power delivery. That limits the choice to small 2x3W amplifier and speakers
* like [PAM8403](https://botland.com.pl/czujniki-dzwieku/12806-wzmacniacz-audio-stereo-pam8403-5v-3w-dwukanalowy-czerwony-5903351241106.html)


2nd version (if ever)

Input - USB-C __with__ power delivery. Amplifier can be high power, something like >10 Watts. Should be fun.
