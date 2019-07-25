## example of client

app.js

```
const socket = io("http://localhost:3000");
window.socket = socket;

// console.log(socket);
//   socket.emit("roomCheck", { message: "room check" });

socket.on("messageTclient", ({ chat }) => {
  console.log(chat);
});
```
