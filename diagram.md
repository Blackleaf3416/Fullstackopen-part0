```mermaid
sequenceDiagram
actor User
participant Browser
participant Server
User->>Browser: write a word in the form
User->>Browser: click on "save"
browser->>server: Send the form to https://studies.cs.helsinki.fi/exampleapp/new_note
server->>browser: Status Code 302
browser->>server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/notes
  
  
```
