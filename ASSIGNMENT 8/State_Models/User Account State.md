## User Account State Diagram

```mermaid
stateDiagram-v2
[*] --> LoggedOut

LoggedOut --> LoggedIn : Login
LoggedIn --> Locked : Invalid Attempts
Locked --> LoggedOut : Reset Password
LoggedIn --> LoggedOut : Logout
```
