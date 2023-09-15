```mermaid
sequenceDiagram
    participant browser
    participant server
    
    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    server-->>browser: [{"content": "spa testi","date": "2023-09-15T17:28:19.664Z"}]
    deactivate server

    Note right of browser: Selain lähettää lomakkeen tiedot POST metodia käyttäen JSON-muodossa. JavaScript-koodi estää lomakkeen<br> normaalin lähettämisen, luo ja lisää uuden muistiinpanon notes taulukkoon ja piirtää listan uudelleen.

```