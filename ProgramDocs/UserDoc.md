# Vehicle JSON Generator App – User Documentation
**Version**: VJG_02JUN25_A  
**Date**: 2025-06-02

## Overview
This guide explains how to operate the Vehicle JSON Generator (VJG) to create JSON vehicle files formatted for Swarm Commander.

MATLAB R2024b or compatible MATLAB Runtime
-  No internet connection required once installed

## Basic Steps to Use the App
1.	Open MATLAB
-  Ensure you're using R2024b or later.
2.	Open the App File
-  Locate and open VehicleJSONGenerator.mlapp using MATLAB App Designer.
3.	Run the App
-  Click the Run button in App Designer.
4.	Use the GUI
-  Select Category: Choose a category (e.g., Combat, UAV) from the top dropdown.
-  Select Variant: Choose a predefined model from the second dropdown.
-  Edit Parameters: (Optional) Adjust speed, weight, or other parameters.
5.	Export the Vehicle
-  Click the Export button. This opens a file explorer.
-  Choose the folder and specify a unique file name (optional).
-  Click Save to create the JSON file.

---

## Features
- **Category Selection**: Choose from Combat, Combat Support, or Combat Service Support vehicles.
- **Dynamic Vehicle Fields**: Automatically populate fields based on selected vehicle.
- **UAV Configuration**: Includes fields specific to UAVs such as altitude and subcategory.
- **Weapon System Specification**: Configure equipped weapon types and related power settings.
- **Image Preview**: Displays vehicle image based on selection.
- **Import/Export Functionality**: (Reserved for future) Import/export configurations to/from JSON files.
- **Reset Function**: Clear all vehicle-related fields with one click.

---

## Getting Started

### Launch the App
Use the following command in MATLAB:
```matlab
app = VJG_02JUN25_A;

