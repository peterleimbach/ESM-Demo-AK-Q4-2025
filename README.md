# ESM-Demo-AK-Q4-2025

```mermaid
sequenceDiagram
    autonumber
    participant Client
    participant Server

    Client ->> Server: POST Login
    Server -->> Client: Session ID
    Client ->> Server: POST Activate - Overview
    Server -->> Client: Activate - Overview
    Client ->> Server: POST Activate - On Hold
    Server -->> Client: Activate - - On Hold
    Client ->> Server: Activate - Release
    Server -->> Client: PUT Activate - Release
    Client ->> Server: DELETE - Logoff
    Server -->> Client: Message "Logoff"
```
