# Class Diagram
Warehouse IT Asset Tracking System

```mermaid
classDiagram

class Asset {
    -assetId: String
    -type: String
    -serialNumber: String
    -status: String
    -location: String
    +register()
    +updateStatus()
    +updateLocation()
}

class User {
    -userId: String
    -name: String
    -email: String
    -role: String
    +login()
    +logout()
}

class Admin {
    +manageAssets()
    +generateReports()
}

class Technician {
    +repairAsset()
}

class FaultReport {
    -reportId: String
    -description: String
    -status: String
    -date: Date
    +createReport()
    +updateStatus()
}

class MaintenanceRecord {
    -recordId: String
    -date: Date
    -description: String
    -status: String
    +addRecord()
}

class Location {
    -locationId: String
    -name: String
    +updateLocation()
}

User <|-- Admin
User <|-- Technician

Asset "1" -- "0..*" MaintenanceRecord : has
Asset "1" -- "0..*" FaultReport : generates
FaultReport "0..*" -- "1" Technician : handled by
Asset "1" -- "1" Location : located at
User "1" -- "0..*" FaultReport : creates
```


## Design Decisions

- Inheritance is used where Admin and Technician extend User.
- Composition is shown between Asset and MaintenanceRecord.
- Associations represent interactions between entities.

### Alignment

This diagram aligns with:
- FR1 (Asset Registration)
- FR5 (Maintenance Tracking)
- FR8 (Fault Reporting)
- Use Cases (Assignment 5)
- State Diagrams (Assignment 8)

### Key Design Choices

- Simplified class structure to maintain clarity.
- Focus on core system functionality.
- Avoided over-complication while maintaining completeness.





