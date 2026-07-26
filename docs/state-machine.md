# State Machine

## Overview
This project uses a simple state-machine structure to control the automatic windshield sunshade system.

The system reads sensor values, determines the current condition, and changes its behavior based on the current state.

## States

| State | Description |
|---|---|
| IDLE | System is waiting and monitoring sensor values |
| HOT_SUNNY | High temperature and strong sunlight are detected |
| DEPLOYING | Sunshade is being deployed |
| DEPLOYED | Sunshade is fully deployed |
| RETRACTING | Sunshade is being retracted |
| MANUAL_MODE | User controls the sunshade manually |
| ERROR | Abnormal sensor value or motor operation failure |

## Basic Transitions

| Current State | Condition | Next State |
|---|---|---|
| IDLE | Temperature is high and light level is high | HOT_SUNNY |
| HOT_SUNNY | Auto mode is enabled | DEPLOYING |
| DEPLOYING | Deployment is complete | DEPLOYED |
| DEPLOYED | Temperature or light level decreases | RETRACTING |
| ANY | Manual button is pressed | MANUAL_MODE |
| ANY | Sensor value is abnormal | ERROR |
| ERROR | Reset button is pressed | IDLE |

## MVP Logic

1. Read temperature sensor value
2. Read light sensor value
3. Check manual button input
4. Decide current state
5. Control motor or servo based on state
6. Display state using LED, LCD, or OLED

## Example Condition

The sunshade may deploy when both conditions are true:

- Temperature is above the defined threshold
- Light level is above the defined threshold

## Future Improvements

- Add limit switches to detect fully deployed/retracted positions
- Add rain sensor condition
- Add parking-state detection
- Add motor timeout protection
- Add safety lock while driving
