# Pico Motorcycle Dashboard (DRAFT)
[![License: GPLv3][GPLimg]][GPLurl]
[![GitHub Tag][GHTimg]][GHTurl]

### A Motorcycle Dashboard based on the [Raspberry Pi Pico](https://www.raspberrypi.org/products/raspberry-pi-pico/) and the [Pimoroni Pico Display Pack](https://shop.pimoroni.com/products/pico-display-pack)

## Components
- Raspberry Pi Pico
  - Main control board
- Pico Display Pack
  - Input:
    - Button A
    - Button B
    - Button X
    - Button Y
  - Output:
    - 240x135 px IPS display
    - RGB LED
- Sensors
  - Built-in temperature sensor
    - (internal ADC on pin 4)
  - DS18B20 Temperature sensor
    - (currently up to 3 in parallel)
- Work in progress
  - Connection for Battery/Fuel/Rpm readings

## Wiring Diagram
### Breadboard - Full diagram
![Breadboard](https://lh3.googleusercontent.com/pw/AM-JKLXL85_Idbb3gWbf9R2kGnM6V2rCgni5Bkqi5iXfEr17kTAaiILxOcSAr_75dyG5yG6MaF1wZdk9zgJaEIjLYNVVo-oQGpdGmY1BgSLjT5BdzeRqhGC0syIUG0vCKQ-imdqL0K-JVeibcEyUr8TJiZcICQ=w800-no)

### Breadboard - Display directly mounted on the back of the Pico (not shown)
![Breadboard](https://lh3.googleusercontent.com/pw/AM-JKLXWoQoD3HZGN70OeTc5_Na8nTq_L9OXpzibpURABGSUnXlKnmc6hwwnwCy0SY2BShxQEjVEbhL1lXR4hClP1XQTbvh8qdTayrBOYNnw01wWPMPRMJ5bonOsW2U9a5SRWykPReBykW9vxZG9WMsQD7OGFw=w800-no)

---
## Usage

## Screens
- [Home](#home)
- [Battery](#battery)
- [Fuel](#fuel)
- [Temperature](#temperature)
- [RPM](#rpm)
- [STATS](#stats)

### Home
![Home](https://lh3.googleusercontent.com/pw/ACtC-3fY9eTrfeXZWzNof3XDhlGW4b0iINYiCK-arYHpiaK88f8zIZf4uVtTmwLXD-MLb32lzvW6lec1UicTL3cPUCY_-cxZ3S_L31h9lXh_ZYtvAxzrkHlZ4aJ4AoH3m6Uu3duIu12AwbdDtfm1ebb0GLGcgw=s360-no)
- A: Go to next (Battery) screen
  - If pressed again within 3 seconds,  
    cycle through all the screens
- B: Cycle Brightness presets, frees memory
- X: Select Multiple or Single Temperature mode
- Y: If Multiple (*) or Single (**) Temperature mode:
  - Cycle Temperature sources (**)
  - Cycle bars style (*) (globally)
- X+B: Cycle Colour palette
- Y+B: Show Info scroll banner (hold)

### Battery
![Battery](https://lh3.googleusercontent.com/pw/ACtC-3cRZARVqOj3eLK5HT7IEDH3oCYMBrJzV4IoWjkwxWfUzRoq7lWQxgcGSRjmvslOcRkJf_uW_Sdo6ap8LsXDHEeFBLG9Z9mpcQSjHWTzUqFLHen39trysQos4LUzx7lbxWpI1GizDKkDiM-RH9BDpUiKWg=s360-no)
- A: Go to Home screen
- B: Cycle Brightness presets, frees memory
- X: Continuous / Discrete battery representation
- Y: Cycle Graphics style
- Y+B: Show Info scroll banner (hold)

### Fuel
![Fuel](https://lh3.googleusercontent.com/pw/ACtC-3d7aUP9n-YRlb5fsQiasavigt714aPAeRD7GU68PknZSBcmQNHQT0gwDpSYR_YjRP1dSf8yflQwINJtYklD0VDCdsSYpglslzOmpUgbf4kJoRtjDThOLJEhuTSJ7TfcW4AJs2xkhtPTBlDIq1NlBzDNAg=s360-no)
- A: Go to Home screen
- B: Cycle Brightness presets, frees memory
- X: -
- Y: Cycle Bars style (globally)
- Y+B: Show Info scroll banner (hold)

### Temperature
![Temperature](https://lh3.googleusercontent.com/pw/ACtC-3coIj2x-SY4z49AYYzUJ3evlu42Rx1Y3xH_y1HIIIZiQ3ibLfleVxyZkxa3Ut2fy_180udtPBvJxI8quuaL5al4tQaowoahNqSa8kXINlJnDUQf5fyY7LQvsKse6ElqJzbGJ1bWASWyciXLHtaTbubgnA=s360-no)
- A: Go to Home screen
- B: Cycle Brightness presets
- X: Cycle Temperature sources
- Y: Clear history for the current temperature source
- Y+B: Show Info scroll banner (hold)

### RPM
![RPM](https://lh3.googleusercontent.com/pw/ACtC-3c_I22cnapZiIY0lHnfPxvrPQy21NtyiYpFDa4_dSBl648UofLTzzr9HfIoObmCWqJxcgv_a8cuPvcN9oUpI8is89dyV_Uw855apra5aaxx1Xd9MiwaeomLO9Rl2M_8R49kOouLLNBiRTrSAAJlZLwvVg=s360-no)
- A: Go to Home screen
- B: Cycle Brightness presets, frees memory
- X: Cycle Ramp style
- Y: Cycle Bars style (globally)
- Y+B: Show Info scroll banner (hold)

### Stats
![Stats](https://lh3.googleusercontent.com/pw/ACtC-3dVguPgP7rk9ptkmF1MP5YwwX98OmDm8XHYJYvoPkmUOCD0PzqJklYjjDLlXXmitVA3WT6abCaqWDLYhKK0s453_RgzQXyZeOpaOMzo3ucDMo3LDURMm4J5ILmOYr5Vfcd4PZfm2JuK_cuEOY3sB7S9iA=s360-no)
- A: Go to Home screen
- B: Cycle Brightness presets, frees memory
- X: Update Configuration file
- Y: Reset uptime
- X+B: Reset Configuration file
- Y+B: Show Info scroll banner (hold)


[GPLimg]: https://img.shields.io/badge/License-GPLv3-blue.svg
[GPLurl]: https://www.gnu.org/licenses/gpl-3.0
[GHTimg]: https://img.shields.io/github/tag/slabua/PicoMotorcycleDashboard.svg
[GHTurl]: https://github.com/slabua/PicoMotorcycleDashboard/tags
