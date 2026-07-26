# Project Plan

## Project Name
Arduino-Based Automatic Windshield Sunshade System

## Korean Name
Arduino 기반 차량 전면유리 자동 차광 시스템

## Problem
In summer, vehicles parked outdoors can heat up quickly due to direct sunlight entering through the windshield.

## Goal
Build a model-based Arduino system that detects sunlight and temperature conditions and automatically controls a sunshade.

## MVP Features
- Measure light level
- Measure temperature
- Deploy or retract the sunshade
- Manual control button
- Display current system state
- Define basic system states

## Basic System Flow
1. Read light sensor value
2. Read temperature sensor value
3. Decide whether shading is needed
4. Control servo motor or DC motor
5. Display current state using LED, LCD, or OLED

## Not Implemented in MVP
- Real vehicle installation
- Full dual-roll mechanical structure
- Vehicle power integration
- Driving-state detection
- Weatherproof exterior hardware

## Future Expansion
A dual-roll structure may allow the sunshade to be automatically deployed and retracted without requiring the user to manually roll it back.

Possible future improvements:
- Dual-roll mechanism
- Limit switches for position detection
- Rain sensor for automatic retraction
- Parking-state detection
- Safety logic to prevent operation while driving
