sequenceDiagram
  participant browser
  participant server

  browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
  activate server
  server-->>browser: [{content: "ompa vaikee pewi", date: "2024-01-24T10:33:21.674Z"}]
  deactivate server

  Note right of browser: browser posts and fetches the posted JSON from the server and render posted notes
