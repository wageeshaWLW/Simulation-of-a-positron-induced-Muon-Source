# Muon Beam Production and Tracking Simulation

## Introduction

This project aims to simulate the production and tracking of a muon beam. The method involves shooting high-energy positrons at a target to produce muons, with a focus on minimizing beam divergence.

## Experimental Setup

### Components

- **Target**: Reaction site for positrons.
- **Dipole Magnet**: 1-meter long, 1 Tesla.
- **Tracking Detectors**: Silicon pixel detectors with resolutions between 50 to 200 micrometers.

### Layout Constraints

- Compact setup within 20 meters.
- Budget considerations limit the number of detectors and their resolution.

## Simulation Steps

1. Define detector sizes and placements.
2. Generate a synthetic dataset with smeared hits and noise.
3. Develop a tracking algorithm for particles.
4. Calculate muon momentum and angular resolution.

## Implementation Details

### Detector Sizes and Placement

- Detectors before the target and after the magnet should cover the entire beam cross-section.
- After-target detector should capture all emerging particles.

### Synthetic Dataset

- Simulate events and record hits.
- Apply smearing based on resolution and add Poisson noise.

### Tracking Algorithm

- Use Kalman filter for tracking.
- Implement clustering for shared hits.

### Resolution Calculation

- Compute momentum and angular divergence resolutions.
