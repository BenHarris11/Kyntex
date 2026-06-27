# Kyntex

**Relative tendon stiffness tracking for athletes managing patellar tendon load, recovery, and return-to-sport progression.**

Kyntex is a wearable sensing system that estimates relative patellar tendon stiffness by applying a controlled mechanical stimulus and measuring how the tendon responds.

## Problem

Athletes with patellar tendon pain often rely on subjective feedback such as pain, soreness, and feel when deciding whether to train, rest, or return to sport.

There is currently no simple wearable tool that helps athletes track how their tendon stiffness changes over time.

## Solution

Kyntex is designed to help athletes monitor relative tendon stiffness trends, including:

- baseline tendon stiffness
- left/right tendon differences
- pre-training vs post-training changes
- weekly recovery trends
- return-to-sport progression

## How It Works

1. A controlled mechanical tap is applied near the patellar tendon.
2. Synchronized accelerometers measure the tendon response.
3. Embedded firmware captures timestamped sensor data.
4. Signal processing estimates relative stiffness from wave-delay and response features.
5. The user sees stiffness changes compared to their own baseline.

## Product Vision

Kyntex is not intended to diagnose injury. The goal is to provide athletes and clinicians with a practical way to track tendon stiffness trends over time.

Example outputs:

- "Your right tendon is 12% stiffer than your left."
- "Your tendon stiffness is 8% lower than last week."
- "Post-training stiffness increased compared to your morning baseline."

## Current Status

Kyntex is currently in prototype development.

Current focus:

- actuator and sensor selection
- relative stiffness measurement pipeline
- bench validation using variable-tension materials
- wearable embedded firmware development
- investor/resume-ready demo system

## Technical Prototype

The technical implementation is being developed separately.

**Technical repo:**  
`kyntex-tendon-stiffness-monitor`

Planned technical stack:

- Nordic nRF54L15
- Zephyr RTOS
- synchronized accelerometer sensing
- ADS131M02 / ADS131M08 ADC
- piezo/tapper mechanical excitation
- BLE data streaming
- Python signal-processing validation

## Roadmap

### Phase 1 — Bench Prototype

Validate that the system can detect stiffness changes in elastic materials under different tension levels.

### Phase 2 — Human Feasibility

Measure relaxed vs contracted tendon states, left/right differences, and pre/post exercise changes.

### Phase 3 — Wearable Prototype

Package the system into a wearable patellar tendon device with BLE streaming and app/dashboard visualization.

### Phase 4 — Validation

Compare relative stiffness trends against reference methods or controlled test conditions.

## Disclaimer

Kyntex is an early-stage prototype and is not a medical device. It is not intended to diagnose, treat, or predict injury.
