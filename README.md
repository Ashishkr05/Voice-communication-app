# WebRTC Voice Chat

Group voice chat application based on the [Pion WebRTC Go library](https://github.com/pion/webrtc).

## Features

- Mute/unmute microphone.
- Mute/unmute speaker.
- To join a room, simply write anything after a slash, e.g., `/myroom`, `/123`, `/test`, etc.

## Demo


### Home Page
![Landing home page](https://github.com/Ashishkr05/Voice-communication-app/assets/77094389/b2abd273-2738-4156-b47c-a82132388105)

### Room
![Room](https://github.com/Ashishkr05/Voice-communication-app/assets/77094389/80e820aa-a1d2-4e9a-bd4d-e7689eb777e9)

## Installation and Running

To start the frontend, run `npm start`. For the backend, execute the appropriate GoLang run `go run main.go`.

## Design Choices

- Created a basic user interface using Next.js allowing users to enter their names and join voice chat rooms.
- Implemented real-time communication using WebSockets for live voice data transmission.
- Managed and displayed the list of users currently connected to the room.
- Utilized GoLang for the backend server, employing WebSockets for real-time voice data exchange.
- Employed Go routines for efficient handling of multiple users and data streams concurrently.

## Challenges Faced and Solutions

- **Real-time Communication:** Ensuring seamless real-time communication between users posed a challenge. This was overcome by implementing robust WebSocket handling and optimizing data transmission.
- **Concurrency Management:** Managing multiple user connections concurrently required careful consideration of Go routines and synchronization. This was addressed by implementing efficient Go routines and proper synchronization mechanisms.
