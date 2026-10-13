# Design and modules

[中文](design.md) | English

## Goal

Start with single-axis software simulation, develop a vision-following gimbal with position feedback, then evaluate a two-axis extension.

Data path: Target observation → freshness and confidence checks → target error → controller → saturation / limits → actuator → position feedback

| Module | Responsibility |
| --- | --- |
| observation | Target location, frame size, capture time and freshness; record reception time. |
| controller | Map error to velocity/position commands; define sample period, deadband, saturation and integral limits. |
| actuator | Driver adaptation, position feedback, limits and stop behavior. |
| behavior | IDLE / TRACK / LOST / STOP; start disabled and enter a stop policy when observations become invalid. |

## Draft interface

Candidate observation fields: target_id, frame_id, image_size, bbox, confidence, capture_time, receive_time. Do not directly subtract clocks from different nodes; begin with local reception timeouts. Pixel error is not a mechanical angle without calibration. Control outputs must declare units and expiry.

This contract has no validated implementation yet. Add examples, edge cases and migration notes when freezing it.

## Scope

Do not retrain a general-purpose detector or jump directly from a bare brushless motor to an integrated system. Do not power hardware before the actuator, driver, feedback and limits are defined.

## Open decisions

- Pin dependency versions and confirm compatibility.
- Use initial measurements to set numerical acceptance thresholds.
- Confirm available hardware and resource budgets.
