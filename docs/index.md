# Kyntex

**Relative tendon stiffness tracking for athletes managing patellar tendon load and recovery.**

Kyntex is a wearable sensing system that estimates relative patellar tendon stiffness by applying a controlled mechanical stimulus and measuring how the tendon responds.

## The Problem

Athletes with jumper's knee often rely on pain, feel, and guesswork to decide when to train, rest, or return to sport.

## The Product

Kyntex helps athletes track how their tendon stiffness changes over time:

- baseline tendon stiffness
- left/right stiffness difference
- pre/post training stiffness change
- weekly recovery trends

## How It Works

1. A controlled mechanical tap is applied near the patellar tendon.
2. Synchronized accelerometers measure the response.
3. Firmware streams timestamped data over BLE.
4. Signal processing estimates relative stiffness from wave-delay and response features.

## Technical Prototype

The current embedded prototype uses:

- Nordic nRF54L15
- synchronized accelerometer sensing
- ADS131M02 / ADS131M08 ADC
- piezo/tapper excitation
- Python validation pipeline

[View the technical repository](https://github.com/BenHarris11/Kyntex-Technical)

## Status

Prototype in development.
