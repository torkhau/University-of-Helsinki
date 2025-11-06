```mermaid
sequenceDiagram
    participant browser
    participant server

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    Note right of browser: Request payload: {"content":"torkhau SPA","date":"2025-11-06T18:43:44.956Z"}.
    activate server
    server-->>browser: Status code: 201 Created.
    deactivate server    
    Note right of browser: Response data: {"message":"note created"}
```