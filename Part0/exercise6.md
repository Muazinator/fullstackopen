# Exercise 6
:::mermaid
sequenceDiagram
    participant browser
    participant server
    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    server-->>browser: HTTP Status code 201 (Created)
    Note right of browser: the server receives the data in json format
    deactivate server
:::s