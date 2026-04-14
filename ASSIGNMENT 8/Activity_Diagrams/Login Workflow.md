## Login Workflow

```mermaid
flowchart TD

Start --> EnterCredentials
EnterCredentials --> Validate
Validate -->|Valid| AccessGranted
Validate -->|Invalid| AccessDenied
AccessGranted --> End
AccessDenied --> End
```
