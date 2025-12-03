# Australian Aged Care Contact Matrix

## Overview
The model simulates staff–resident interactions in a synthetic aged care facility. It generates proximity-based contact events across:
  - Residents: high care, medium care, and low care categories
  - Staff: morning, afternoon, and night shifts

A contact event is defined as two agents being within:
  - 1.5 m or
  - 3.0 m,
  for a duration of ≥ 3 seconds.

The primary purpose of the model is to generate empirically grounded contact matrices that reflect heterogeneity in resident care needs and staff shift structures. These contact matrices are used for epidemiological and transmission modelling.

<p align="center">
  <img src="assets/Visual Pipeline ABM.jpeg" alt="framework" width="760">
</p>

## Model Description 
The model simulates daily operations in an aged care facility using AnyLogic’s pedestrian library and custom Java code. It includes:

- A spatial layout of bedrooms, bathrooms, communal rooms, transit corridors, and service areas
- Resident behaviour routines (movement, activities, resting periods)
- Staff workflows, handover processes, and scheduled shift changes
- Priority-based navigation and congestion-dependent movement
- Dynamic tracking of distances between all agent pairs at 1-second resolution
- Generation of individual-level contact logs and aggregated matrices

The model is non-stochastic in layout but stochastic in movement, activity choices, and timing.

## Usage
With AnyLogic 8
  - Open AgedCareContactModel.xml in AnyLogic (v8.9 or later).
  - Clone or download this repository.
  - Open AgedCareContactModel.xml and run the main agent
Without AnyLogic
  - The XML file can be inspected directly as structured text.
  - A documentation-style summary may be added in the future for easier interpretation.
