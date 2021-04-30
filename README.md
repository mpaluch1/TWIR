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
* I2S DAC - for dat sound quality
* Energy efficient audio amplifier if not present in above
* Some kind of USB-C IC
* Some kind of speakers
