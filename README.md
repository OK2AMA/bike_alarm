# bike_alarm
Battery powered, radio two way, bike alarm. 
Divided into two parts:
- cable lock alarm
   - Canon 9 pin (RS232) cable, with "special connection"
      - because of low quiscent current
   - Inside:
      - LoRa, ESP8266/Arduino, 18650 cell, horn
   - event levels:
      - 1 silent alarm, led blink
      - 2 after 5 sec, short horn
      - 3 cable intrupts, horn, 
- bike onboard alarm
   - horn in outside area of motorbike
   - mercury angle switch sensor
   - (MPU not used)
- user hanheld unit 
   - to report alarm events

# Main characteristics
- battery powered
   - 18650 lion,
   - horn step up converter?
- mercury tilt switches to interrupt microcontroller
- lora RF module to inform bike owner in case of alarm on
- if alarm event ocure, it save Bluetooth ID in neighborhood
   - black list - silent alarm if somebody from blacklist is close 
