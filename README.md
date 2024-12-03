# HomePLC-AlarmManager

TwinCAT library for an alarm manager that is part of the HomePLC library.

## Dependencies

- [HomePLC DIO](https://github.com/irtom/HomePLC-DIO)
- [HomePLC Logging](https://github.com/irtom/HomePLC-Logging)

## Required hardware

The library works with the following hardware:

- Keypads
  - 6 Keys (digital inputs)
  - 6 LEDs (digital outputs)
  - 1 buzzer (digital output
- Sensors
  - Detection signal (digital input)
  - Tamper input (digital input)
- Sirens
  - Siren sound (digital output)
  - Siren light (digital output)
  - Tamper input (digital input)
 
## Contents

- FB_AlarmManager
  - Combines the functionality of the keypad(s), sensor(s) and siren(s)
  - Contains a state machine that enables and disables the alarm, monitors sensors, sounds the siren, etc.
- FB_AlarmKeypad
  - Shows whether the alarm is enabling, on, etc.
  - Allows the user to input the alarm code
- FB_AlarmSensor
  - Reports when motion is detected
  - Reports when the sensor is tampered with
- FB_AlarmSiren
  - Alerts the user when the alarm is triggered by sound and light
  - Reports when the siren is tampered with

## Example usage
See the [example repository](https://github.com/irtom/HomePLC-Example).
