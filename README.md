# EcoCAR EVC Y2 Fall Workshop CI/CD Training

This repository contains an example model of a thermal control system for use with the 2023 EcoCAR Fall Workshop CI/CD training sponsored by Our Next Energy (ONE) and dSPACE.

## Overview

### Models

This repository contains a model called `models/thermostatController.slx`, which represents a thermostat controller.

A sim harness is provided with a basic simulation of a room located at `harness/thermostatController_SimHarness.slx`.

### Scripts

This repository contains several MATLAB scripts to setup the simulation and PI controller tuning.

- `pid_1.m` - One possible tuning for the PI controller.
- `pid_2.m` - One possible tuning for the PI controller.
- `pid_3.m` - One possible tuning for the PI controller.
- `setupPID.m` - A script to call the appropriate PID tuning script.
- `thermal_data.m` - A script containing thermal simulation data for the sim harness.

### Tests

This repository includes a Simulink test suite test suite with two tests.

- PI Controller Tests
  - Overshoot - Tests the thermostat PI controller overshoot.
  - Rise Time - Tests the rise time for the PI controller.

## Contributors

- Lukas Lemke (dSPACE) - Creator of the model.
- Sam Reinsel (MathWorks) - Added tests for workshop.
- Kirk Brauer (ONE) - Tested with CI/CD workflows.
