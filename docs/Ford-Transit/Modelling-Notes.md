# Ford Transit 350 L3H3 AWD MK8 Modelling Notes

## Overview

This document defines the modelling workflow and standards for the:

**Open Transit Project (OTP)**

**Ford Transit 350 L3H3 AWD MK8 - Right-Hand Drive (RHD) Digital Twin**

The purpose of this document is to ensure that all 3D development remains:

- Accurate
- Scalable
- Organised
- Editable
- Reusable

---

# Modelling Goals

The digital twin should represent the vehicle accurately for:

- Blueprint generation
- Interior design
- Conversion planning
- Visualisation
- Simulation
- Asset export

The primary modelling focus is:

1. Exterior body accuracy
2. Cargo area accuracy
3. Interior structure
4. Component detail

---

# Blender Project Standards

## Software

Primary software:

- Blender

Recommended version:

_To be confirmed_

---

# Scene Setup

## Units

Use:

- Metric units
- Metres as the base unit

Recommended settings:

Unit System: Metric
Length: Metres
Scale: 1.0


---

# Coordinate System

The vehicle should use a consistent world orientation.

## Axis Convention

| Axis | Purpose |
|---|---|
| X | Vehicle length |
| Y | Vehicle width |
| Z | Vehicle height |

---

# Vehicle Origin

Recommended origin point:

- Vehicle centreline
- Front axle reference
- Ground plane alignment

Reference:

X = Vehicle length position
Y = Centreline
Z = Ground level


---

# Scene Organisation

Recommended collection structure:

FORD_TRANSIT_MK8_L3H3

├── 00_REFERENCE
│
├── 01_BODY
│
├── 02_GLASS
│
├── 03_INTERIOR
│
├── 04_CHASSIS
│
├── 05_MECHANICAL
│
├── 06_ELECTRICAL
│
├── 07_DETAILS
│
├── 08_MATERIALS
│
└── 09_EXPORTS


---

# Object Naming Convention

All objects should use clear names.

Format:

FT_[SYSTEM][PART][VERSION]

Examples:

FT_BODY_FRONT_PANEL_V01

FT_DOOR_SLIDING_RIGHT_V01

FT_WHEEL_FRONT_RIGHT_V01


---

# Modelling Workflow

## Phase 1 - Reference Setup

Create:

- Blueprint planes
- Reference images
- Measurement guides
- Vehicle centreline

---

## Phase 2 - Base Vehicle Shape

Model:

- Overall body volume
- Roof height
- Wheel arches
- Major panels

Priority:

Correct proportions over detail.

---

## Phase 3 - Exterior Details

Add:

- Doors
- Windows
- Mirrors
- Lights
- Handles
- Trim

---

## Phase 4 - Cargo Area

Primary project focus.

Model:

- Floor
- Side walls
- Roof structure
- Door openings
- Wheel arches
- Structural ribs

---

## Phase 5 - Interior

Model:

- Dashboard
- Steering wheel
- Seats
- Cab trim
- Storage areas

---

# Mesh Standards

Models should maintain:

- Clean topology
- Editable geometry
- Logical edge flow
- Applied scale
- Correct normals

Avoid:

- Unnecessary subdivision
- Hidden geometry
- Duplicate objects

---

# Materials

Materials should be organised by vehicle system.

Examples:

MAT_BODY_PAINT
MAT_GLASS
MAT_RUBBER
MAT_METAL
MAT_PLASTIC
MAT_INTERIOR


---

# Reference Image Workflow

Reference images should include:

- Correct scale
- Known dimensions
- Alignment points

Recommended views:

- Front
- Rear
- Left side
- Right side
- Top
- Interior

---

# CAD Workflow

CAD references should be:

1. Imported
2. Checked against known dimensions
3. Scaled correctly
4. Locked as reference layers

---

# Export Standards

Supported export formats:

- Blender (.blend)
- FBX
- OBJ
- glTF

Before export:

Check:

- Scale
- Origin
- Materials
- Object names
- Applied transforms

---

# Version Control

Major milestones should be saved as:

FORD_TRANSIT_MK8_L3H3_V001
FORD_TRANSIT_MK8_L3H3_V002


Each version should include notes describing changes.

---

# Development Notes

Record:

- Modelling decisions
- Assumptions
- Measurements used
- Known inaccuracies

---

# Revision History

| Date | Change | Author |
|---|---|---|
| Initial | Created modelling framework | Open Transit Project |


