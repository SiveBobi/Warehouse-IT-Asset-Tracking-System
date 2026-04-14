# Activity Diagrams

## Register Asset Workflow

```mermaid
flowchart TD

Start --> EnterDetails
EnterDetails --> Validate
Validate -->|Valid| Save
Validate -->|Invalid| Error
Save --> End
Error --> End
```
