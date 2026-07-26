# Components

## Required Components

| Component | Role | Purpose |
|---|---|---|
| Arduino UNO R3 | Main controller | Controls sensors and actuators |
| Breadboard | Circuit prototyping | Connect components without soldering |
| Jumper wires | Wiring | Connect Arduino and modules |
| Resistors | Circuit protection | Protect LEDs and input circuits |
| Light sensor | Input sensor | Detect sunlight intensity |
| Temperature sensor | Input sensor | Measure surrounding temperature |
| Button | User input | Manual deploy/retract control |
| Servo motor | Actuator | Simulate sunshade deployment |
| LED | Status output | Show system state |
| LCD or OLED display | Status display | Show temperature, light level, and state |

## Optional Components

| Component | Role | Purpose |
|---|---|---|
| Buzzer | Warning output | Alert error or state change |
| Limit switch | Position sensor | Detect fully deployed/retracted position |
| Rain sensor | Input sensor | Retract sunshade when rain is detected |
| DC motor | Actuator | More realistic roll mechanism |
| Motor driver | Motor control | Control DC motor safely |
| Battery pack | Power supply | Portable testing |

## MVP Component Choice

For the first version, the system will likely use a servo motor instead of a DC motor.  
A servo motor is easier to control and more suitable for a model-based MVP.

## Future Component Ideas

- Dual-roll structure
- DC motor with motor driver
- Limit switches
- Rain sensor
- Stronger frame structure
- Realistic windshield model
