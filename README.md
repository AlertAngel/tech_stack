# Tech Stack 

The tech stacks planned on being used 

## Hardware

The hardware planned on being used are as follows : 
1. ESP32 Microcontroller (ESP32-WROOM)
2. 2.4" TFT display Monitor
3. MPU9250 Inertial Measurement Unit
4. MAX30102 Pulse Oximeter and Heart rate monitor
5. DS18B20 temperature sensor module
6. Pushbuttons

## Firmware

For the Embedded firmware, Rust (`std`) seems to be a very good option due to it's architecture and inbuilt memory safety. 

Due to the lack of a garbage collector, it prevents buffer overflows.

### Firmware Crates

1. `esp_idf_svc` : ESP-IDF framework for Rust (`std`)
2. `hayasen` : Sensor Library (For MPU9250 and MAX30102) senors
3. `onewire` : Library to read the temperature from a DS18B20 Temperature sensor
4. `mousefood` : `embedded-graphics` backend for `ratatui`
5. `ratatui` : Library for cooking up Terminal User Interfaces (TUI's)
6. `mpipdsi` : Library for using the TFT screen.

## Third Party `ratatui` crates

These are some 3rd-part `ratatui` crates that can be used for better aesthetics

1. `tui-big-text`
2. `tui-popup`
3. `tui-piechart`
