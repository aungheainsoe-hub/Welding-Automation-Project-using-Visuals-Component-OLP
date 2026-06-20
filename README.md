# Welding Automation with Visual Components OLP

Offline-programmed, multi-sequence robotic welding cell built and simulated in
Visual Components OLP 10, with programs generated for a Yaskawa Motoman robot.

## Overview
This project develops an automated welding workflow covering multiple weld types
across a single multi-step sequence. The cell was modelled and simulated offline,
and robot programs were generated and verified in simulation before any real-world
deployment — the core value of offline programming (OLP).

## Tools & methods
- Visual Components OLP 10 (3D simulation + offline programming)
- Yaskawa Motoman robot (INFORM / `.JBI` job files)
- Weld sequencing, reachability and collision checking, cycle verification

## The sequence
The workflow is split into steps, each exported as a robot job:
- `HOME.JBI` — home / safe position
- `L_F_TOP_1_S1.JBI` — fillet weld, top, step 1
- `L_F_BOTTOM_S2.JBI` — fillet weld, bottom, step 2
- `CIRCULAR_S3.JBI` — circular weld, step 3
- `FACE_S4.JBI` — face weld, step 4
- `SEQUENCE1.JBI` — combined multi-step sequence

## Repository contents
- `*.JBI` — Motoman robot job programs (INFORM language)
- `Welding_Automation_Project.pdf` — full project report
- `optimized.vcmx` — Visual Components project 

