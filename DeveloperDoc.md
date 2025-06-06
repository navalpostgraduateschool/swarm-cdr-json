
---

### 🛠️ **Developer Documentation** (`Developer_Documentation.md`)

```markdown
# Vehicle JSON Generator App – Developer Documentation
**Class**: VJG_02JUN25_A  
**Date**: 2025-06-02

## Architecture
App designed using MATLAB App Designer (Class-based, extending `matlab.apps.AppBase`).

### Main Sections
- Vehicle Panel
- UAV Panel
- Weapon System Panel

---

## Core Components

### Properties
- `VehicleData`: Struct storing default configurations for each vehicle.
- `VehicleNameMap`: Maps dropdown display names to struct field keys.

---

## Callback Functions

### `startupFcn(app)`
- Initializes default vehicle configurations under `VehicleData`.
- Categories include `combat`, `combatsupport`, `combatservicesupport`.

### `CategoryDropDownValueChanged(app, event)`
- Updates vehicle list based on category.
- Maps UI labels to struct field keys and stores in `VehicleNameMap`.

### `VehicleDropDownValueChanged(app, event)`
- Loads selected vehicle's parameters into the UI.
- Loads appropriate image from app's directory.
- Fallback image if file not found.

### `ResetButtonPushed(app, event)`
- Clears values in the vehicle panel.

---

## UI Creation

### `createComponents(app)`
- Creates and initializes all UI elements including labels, buttons, dropdowns, images, and edit fields.

---

## Notes
- Uses `containers.Map` for mapping display names to internal keys.
- `uialert` is used for error handling when a vehicle name is invalid.
- All image files are expected to reside in the same directory as the `.mlapp` or `.m` file.

---

## To Do (Enhancements)
- Implement Import/Export functionality for JSON.
- Add input validation for numeric fields.
- Add error handling for UAV image loading.
