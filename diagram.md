```mermaid
sequenceDiagram
actor User
participant Browser
participant Server
User->>Browser: write a word in the form
User->>Browser: click on "save"
Browser->>Server: POST https://studies.cs.helsinki.fi/exampleapp/new_note
activate Server
Server-->>Browser: Status Code 302 Found
Deactivate Server
Browser->>Server: GET https://studies.cs.helsinki.fi/exampleapp/notes
Browser->>Server: GET https://studies.cs.helsinki.fi/exampleapp/main.css
Server-->>Browser: main.css
Browser->>Server: GET https://studies.cs.helsinki.fi/exampleapp/main.js
Server-->>Browser: main.js
Note right of Browser: The browser starts executing the JavaScript code that fetches the JSON from the server
Browser->>Server: GET https://studies.cs.helsinki.fi/exampleapp/data.json
Server-->>Browser: [
    {
        "content": "",
        "date": "2024-05-06T03:20:53.876Z"
    },
    {
        "content": "love from china",
        "date": "2024-05-06T03:30:14.482Z"
    },
    {
        "content": "",
        "date": "2024-05-06T03:32:37.672Z"
    },
    {
        "content": "",
        "date": "2024-05-06T03:34:49.880Z"
    },
    {
        "content": "Hi",
        "date": "2024-05-06T03:35:40.272Z"
    },
    {
        "content": "hi",
        "date": "2024-05-06T03:35:51.855Z"
    },
    {
        "content": "hello!",
        "date": "2024-05-06T03:56:45.472Z"
    },
    {
        "content": "",
        "date": "2024-05-06T04:06:18.084Z"
    },
    {
        "content": "Hello!",
        "date": "2024-05-06T04:11:45.476Z"
    },
    {
        "content": "Test!",
        "date": "2024-05-06T04:18:22.473Z"
    },
    {
        "content": "Test!",
        "date": "2024-05-06T04:19:10.810Z"
    },
    {
        "content": "Test",
        "date": "2024-05-06T04:19:23.201Z"
    },
    {
        "content": "New note",
        "date": "2024-05-06T05:06:21.538Z"
    },
    {
        "content": "",
        "date": "2024-05-06T05:07:53.809Z"
    },
    {
        "content": "Hi",
        "date": "2024-05-06T05:13:15.524Z"
    },
    {
        "content": "tired",
        "date": "2024-05-06T05:19:09.854Z"
    },
    {
        "content": "Hi",
        "date": "2024-05-06T06:33:47.497Z"
    },
    {
        "content": "",
        "date": "2024-05-06T06:37:27.879Z"
    },
    {
        "content": "Mexico",
        "date": "2024-05-06T06:37:38.290Z"
    },
    {
        "content": "Hello",
        "date": "2024-05-06T06:58:52.608Z"
    },
    {
        "content": "Miten menee?",
        "date": "2024-05-06T07:26:52.686Z"
    },
    {
        "content": "halo",
        "date": "2024-05-06T07:34:50.148Z"
    },
    {
        "content": "Hello",
        "date": "2024-05-06T08:25:56.928Z"
    },
    {
        "content": "test",
        "date": "2024-05-06T08:26:12.549Z"
    },
    {
        "content": "passwords",
        "date": "2024-05-06T08:35:30.489Z"
    },
    {
        "content": "admin",
        "date": "2024-05-06T08:35:39.709Z"
    },
    {
        "content": "webadmin",
        "date": "2024-05-06T08:35:49.361Z"
    },
    {
        "content": "Hola amigos!",
        "date": "2024-05-06T08:39:57.492Z"
    },
    {
        "content": "Hola amigos!",
        "date": "2024-05-06T08:39:57.966Z"
    },
    {
        "content": "dasd",
        "date": "2024-05-06T08:41:20.172Z"
    },
    {
        "content": "Test please",
        "date": "2024-05-06T08:41:30.158Z"
    },
    {
        "content": "Oh looks like this is a good thing",
        "date": "2024-05-06T08:42:03.074Z"
    },
    {
        "content": "Hi",
        "date": "2024-05-06T08:46:14.497Z"
    },
    {
        "content": "test",
        "date": "2024-05-06T08:54:48.320Z"
    },
    {
        "content": "test",
        "date": "2024-05-06T08:54:56.374Z"
    },
    {
        "content": "34",
        "date": "2024-05-06T08:58:32.171Z"
    },
    {
        "content": "hi",
        "date": "2024-05-06T09:03:54.859Z"
    },
    {
        "content": "dsdasd",
        "date": "2024-05-06T09:11:41.325Z"
    },
    {
        "content": "sASa",
        "date": "2024-05-06T09:11:46.953Z"
    },
    {
        "content": "ciao",
        "date": "2024-05-06T09:12:06.853Z"
    },
    {
        "content": "",
        "date": "2024-05-06T09:15:02.107Z"
    },
    {
        "content": "",
        "date": "2024-05-06T09:15:06.399Z"
    },
    {
        "content": "kee",
        "date": "2024-05-06T09:15:20.011Z"
    },
    {
        "content": "thank you",
        "date": "2024-05-06T09:30:20.467Z"
    },
    {
        "content": "Add one",
        "date": "2024-05-06T09:34:54.710Z"
    },
    {
        "content": "Russell Westbrook",
        "date": "2024-05-06T09:50:00.324Z"
    },
    {
        "content": "uwu",
        "date": "2024-05-06T09:59:20.430Z"
    },
    {
        "content": "xczxczxcz",
        "date": "2024-05-06T09:59:37.779Z"
    },
    {
        "content": "Russell Westbrook",
        "date": "2024-05-06T10:09:26.767Z"
    },
    {
        "content": "SDAadsfasdfasdf",
        "date": "2024-05-06T10:14:41.974Z"
    },
    {
        "content": "dfasdfasdfasdfasdwertwertwe345354353",
        "date": "2024-05-06T10:20:08.183Z"
    },
    {
        "content": "jotain",
        "date": "2024-05-06T10:33:17.017Z"
    },
    {
        "content": "ciao",
        "date": "2024-05-06T10:38:15.731Z"
    },
    {
        "content": "你好",
        "date": "2024-05-06T10:50:03.249Z"
    },
    {
        "content": "wood",
        "date": "2024-05-06T11:07:49.659Z"
    },
    {
        "content": "hi from Vietnam",
        "date": "2024-05-06T11:17:14.641Z"
    },
    {
        "content": "hola",
        "date": "2024-05-06T11:19:21.869Z"
    },
    {
        "content": "asasd",
        "date": "2024-05-06T11:19:40.200Z"
    },
    {
        "content": "asasd",
        "date": "2024-05-06T11:19:43.273Z"
    },
    {
        "content": "dfds",
        "date": "2024-05-06T11:28:51.333Z"
    },
    {
        "content": "stock",
        "date": "2024-05-06T11:36:42.364Z"
    },
    {
        "content": "jotain",
        "date": "2024-05-06T11:36:58.863Z"
    },
    {
        "content": "norway",
        "date": "2024-05-06T11:37:03.040Z"
    },
    {
        "content": "two",
        "date": "2024-05-06T11:37:10.499Z"
    },
    {
        "content": "k",
        "date": "2024-05-06T11:37:35.790Z"
    },
    {
        "content": "david foster wallace",
        "date": "2024-05-06T11:46:33.496Z"
    },
    {
        "content": "anass",
        "date": "2024-05-06T11:50:12.848Z"
    },
    {
        "content": "planisphere",
        "date": "2024-05-06T11:54:10.354Z"
    },
    {
        "content": "the beatles",
        "date": "2024-05-06T11:54:27.052Z"
    },
    {
        "content": "anass",
        "date": "2024-05-06T12:00:34.316Z"
    },
    {
        "content": "italia 2024may6",
        "date": "2024-05-06T12:06:07.843Z"
    },
    {
        "content": "Gl -TheQrow",
        "date": "2024-05-06T12:14:48.349Z"
    },
    {
        "content": "hii",
        "date": "2024-05-06T12:45:29.590Z"
    },
    {
        "content": "hii",
        "date": "2024-05-06T12:45:30.442Z"
    },
    {
        "content": "Once Again",
        "date": "2024-05-06T12:51:37.655Z"
    },
    {
        "content": "Russell Westbrook",
        "date": "2024-05-06T12:57:40.644Z"
    },
    {
        "content": "Hello from the other side",
        "date": "2024-05-06T12:59:43.716Z"
    },
    {
        "content": "esta es mi tarea",
        "date": "2024-05-06T13:06:10.266Z"
    },
    {
        "content": "88ii",
        "date": "2024-05-06T13:06:48.251Z"
    },
    {
        "content": "test",
        "date": "2024-05-06T13:07:42.682Z"
    },
    {
        "content": "<h1>test</h1>",
        "date": "2024-05-06T13:18:00.643Z"
    },
    {
        "content": "Russell Westbrook",
        "date": "2024-05-06T13:20:43.076Z"
    },
    {
        "content": "huuuuu",
        "date": "2024-05-06T13:23:39.635Z"
    },
    {
        "content": "hi this is eric",
        "date": "2024-05-06T13:24:17.798Z"
    },
    {
        "content": "Nochmal",
        "date": "2024-05-06T13:28:03.608Z"
    },
    {
        "content": "大家好，我是马楼",
        "date": "2024-05-06T13:32:05.772Z"
    },
    {
        "content": "seba",
        "date": "2024-05-06T13:33:55.557Z"
    },
    {
        "content": "gerg",
        "date": "2024-05-06T13:35:05.340Z"
    },
    {
        "content": "creating the diagram",
        "date": "2024-05-06T13:36:16.551Z"
    },
    {
        "content": "HI from India",
        "date": "2024-05-06T13:37:43.901Z"
    },
    {
        "content": "Hello",
        "date": "2024-05-06T13:42:59.387Z"
    },
    {
        "content": "Hi",
        "date": "2024-05-06T13:43:35.052Z"
    },
    {
        "content": "",
        "date": "2024-05-06T13:51:14.111Z"
    },
    {
        "content": "creating the diagram",
        "date": "2024-05-06T13:54:13.026Z"
    },
    {
        "content": "where are you guys from?",
        "date": "2024-05-06T13:54:25.493Z"
    },
    {
        "content": "earth",
        "date": "2024-05-06T13:55:23.598Z"
    },
    {
        "content": "Mars",
        "date": "2024-05-06T13:56:45.098Z"
    },
    {
        "content": "hello",
        "date": "2024-05-06T14:04:41.249Z"
    },
    {
        "content": "ddddd",
        "date": "2024-05-06T14:05:06.580Z"
    },
    {
        "content": "ty",
        "date": "2024-05-06T14:05:41.122Z"
    }
]
```
