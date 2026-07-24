# Ford Transit 350 L3H3 AWD MK8 Blueprint Workflow

## Overview

This document defines the blueprint creation workflow for the:

**Open Transit Project (OTP)**

**Ford Transit 350 L3H3 AWD MK8 - Right-Hand Drive (RHD) Digital Twin**

The purpose of this workflow is to convert technical references, manufacturer drawings, and measured data into accurate blueprint resources for:

- CAD development
- Blender modelling
- Digital twin construction
- Interior design
- Conversion planning

---

# Blueprint Objectives

The blueprint package should provide accurate references for:

- Exterior body modelling
- Cargo area modelling
- Interior layout
- Component placement
- Scale verification

The final blueprint package should represent the vehicle in true scale.

---

# Required Blueprint Views

## Exterior Views

The following orthographic views should be created:

| View | Purpose |
|---|---|
| Front elevation | Vehicle width, height, front geometry |
| Rear elevation | Rear doors, width, height |
| Left side elevation | Body length and profile |
| Right side elevation | RHD reference side |
| Top plan view | Width, roof shape, component layout |
| Underside view | Chassis and lower structure |

---

## Interior Views

Required internal references:

| View | Purpose |
|---|---|
| Cargo floor plan | Floor dimensions and layout |
| Cargo side elevation | Wall and roof geometry |
| Roof layout | Structural rib placement |
| Door openings | Access dimensions |
| Cab layout | Driver area reference |

---

# Primary Reference Sources

Blueprint creation should prioritise:

1. Ford Body Builder drawings
2. Manufacturer technical specifications
3. Verified vehicle measurements
4. Photographic references

---

# Blueprint Preparation Workflow

## Step 1 - Collect Source Material

Gather:

- Technical drawings
- Dimension tables
- Vehicle photographs
- Inspection measurements

Record all sources in:

Reference-Sources.md


---

## Step 2 - Image Preparation

Before importing:

Check:

- Image quality
- Correct orientation
- Missing information
- Known dimensions

Remove:

- Perspective distortion
- Incorrect scaling
- Unverified overlays

---

# Scaling Process

All blueprint images must be converted to true scale.

## Scale Reference

Primary units:

- Millimetres
- Metres

Recommended Blender scale:

1 Blender Unit = 1 Metre


---

## Scaling Method

1. Identify known vehicle dimension
2. Apply measurement reference
3. Scale image proportionally
4. Lock scale
5. Verify against secondary dimensions

---

# Blueprint Alignment

All views must share common reference points.

## Alignment References

Use:

- Vehicle centreline
- Ground plane
- Wheel centres
- Axle positions
- Door openings

---

# CAD Layer Organisation

Recommended layer structure:

FORD_TRANSIT_BLUEPRINT

├── 00_REFERENCE
│
├── 01_DIMENSIONS
│
├── 02_BODY_OUTLINE
│
├── 03_DOORS
│
├── 04_WINDOWS
│
├── 05_WHEELS
│
├── 06_INTERIOR
│
└── 07_NOTES


---

# SVG Blueprint Workflow

SVG files may be used for scalable technical references.

Recommended uses:

- Floor plans
- Layout drawings
- Dimension overlays
- CAD guides

SVG requirements:

- Real-world scale
- Clear layer names
- No unnecessary paths
- Consistent line weights

---

# Blender Reference Setup

Blueprint images should be imported as:

- Reference objects
- Correctly scaled planes
- Locked background elements

Recommended collections:

00_REFERENCE

├── FRONT_BLUEPRINT
├── REAR_BLUEPRINT
├── LEFT_BLUEPRINT
├── RIGHT_BLUEPRINT
└── TOP_BLUEPRINT


---

# Accuracy Verification

Before modelling begins:

Verify:

## Exterior

- Overall length
- Overall width
- Overall height
- Wheel position
- Door locations

## Cargo Area

- Floor length
- Floor width
- Wheel arch position
- Roof height
- Door openings

---

# Blueprint Revision Control

Each revision should include:

- Date
- Source changes
- Measurement changes
- Accuracy improvements

Naming convention:

FORD_TRANSIT_MK8_L3H3_BLUEPRINT_V001
FORD_TRANSIT_MK8_L3H3_BLUEPRINT_V002


---

# Modelling Handoff

A completed blueprint package should provide:

- Scaled orthographic drawings
- Reference images
- Dimension information
- Alignment points
- CAD-ready guides

These resources become the foundation for:

- Blender modelling
- CAD development
- Digital twin construction

---

# Revision History

| Date | Change | Author |
|---|---|---|
| Initial | Created blueprint workflow framework | Open Transit Project |





