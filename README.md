# Socket.IO Chat
A simple chat demo for Socket.IO

### How to use

$ npm ci

Copy `.env.example` to `.env` and fill in your secrets, then generate a local self-signed certificate:

```bash
openssl req -x509 -newkey rsa:2048 -nodes -keyout certificates/server.key -out certificates/server.cert -days 365 -subj "/CN=localhost"
```

$ npm start

And point your browser to http://localhost:3000. Optionally, specify a port by supplying the PORT env variable.

###Features
Multiple users can join a chat room by each entering a unique username on website load.
Users can type chat messages to the chat room.
A notification is sent to all users when a user joins or leaves the chatroom.