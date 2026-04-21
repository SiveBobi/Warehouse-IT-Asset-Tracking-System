# Domain Model
Warehouse IT Asset Tracking System

## Key Entities

| Entity | Attributes | Methods | Relationships |
|--------|-----------|---------|--------------|
| Asset | assetId, type, serialNumber, status, location | register(), updateStatus(), updateLocation() | Belongs to Location, has MaintenanceRecord |
| User | userId, name, role, email | login(), logout() | Creates FaultReport |
| FaultReport | reportId, description, status, date | createReport(), updateStatus() | Linked to Asset, handled by Technician |
| MaintenanceRecord | recordId, date, description, status | addRecord(), updateRecord() | Belongs to Asset |
| Location | locationId, name | updateLocation() | Contains Assets |
| Technician | technicianId, name | repairAsset() | Handles FaultReports |
| Admin | adminId, name | manageAssets(), generateReports() | Manages Assets |

---

## Business Rules

- An Asset must have a unique ID.
- An Asset can only be in one location at a time.
- A Fault Report must be linked to one Asset.
- A Technician can handle multiple Fault Reports.
- An Asset can have multiple Maintenance Records.
- Only Admin users can register or update assets.
- Fault Reports must be resolved before closure.

---

## Explanation

The domain model represents the core entities involved in the system.

It aligns with:
- Functional Requirements (Assignment 4)
- Use Cases (Assignment 5)
- State Models (Assignment 8)

The relationships ensure that all system interactions are logically connected.
