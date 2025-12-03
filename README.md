# Australian Aged Care Contact Matrix

## Overview
The model simulates staff–resident interactions in a synthetic aged care facility. It generates proximity-based contact events across:
  - Residents: high care, medium care, and low care categories
  - Staff: morning, afternoon, and night shifts
Contacts are defined by thresholds of 1.5 m and 3 m for at least 3 s, forming the basis for contact matrices used in subsequent epidemiological analyses.
<p align="center">
  <img src="assets/Visual Pipeline ABM.png" alt="framework" width="760">
</p>
## Usage
With AnyLogic 8
  - Open AgedCareContactModel.xml in AnyLogic (v8.9 or later).
  - Run simulations to generate staff–resident contacts and contact matrices.
Without AnyLogic
  - The XML file can be inspected directly as structured text.
  - A documentation-style summary may be added in the future for easier interpretation.
