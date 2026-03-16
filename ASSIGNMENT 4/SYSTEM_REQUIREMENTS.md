# System Requirements Document (SRD)
Warehouse IT Asset Tracking System

## 1 Functional Requirements

### FR1: Asset Registration
The system shall allow IT administrators to register new IT assets into the system.

Acceptance Criteria:
- Asset ID must be unique.
- Asset information must include type, serial number, and location.

---

### FR2: Asset Location Tracking
The system shall allow administrators to record and update the location of each asset.

Acceptance Criteria:
- System must display the latest location of the asset.
- Location changes must be logged.

---

### FR3: Asset Status Management
The system shall allow administrators to update the status of equipment.

Statuses include:
- Working
- Faulty
- Under Repair
- Retired

Acceptance Criteria:
- Status updates must be recorded with timestamps.

---

### FR4: Asset Search
The system shall allow users to search assets by asset ID, type, or location.

Acceptance Criteria:
- Search results must display within 2 seconds.

---

### FR5: Maintenance Records
The system shall record maintenance history for each asset.

Acceptance Criteria:
- Each repair must include date, technician, and repair description.

---

### FR6: Asset History Tracking
The system shall maintain a complete history of asset movements and repairs.

Acceptance Criteria:
- History logs must not be editable after creation.

---

### FR7: Asset Reporting
The system shall generate reports on asset status and usage.

Acceptance Criteria:
- Reports must be downloadable in PDF or CSV format.

---

### FR8: Fault Reporting
Warehouse staff shall be able to report faulty equipment.

Acceptance Criteria:
- Fault report must include asset ID and description.

---

### FR9: Notifications
The system shall notify IT administrators when equipment is reported faulty.

Acceptance Criteria:
- Notifications must be sent immediately after reporting.

---

### FR10: User Authentication
The system shall allow administrators to log in securely.

Acceptance Criteria:
- Users must enter valid username and password.

---

### FR11: Asset Dashboard
The system shall display a dashboard showing all assets and their current status.

Acceptance Criteria:
- Dashboard must show summary statistics of assets.
