// WebSocket Server তৈরি
const WebSocket = require('ws');
const wss = new WebSocket.Server({ port: 8080 });

wss.on('connection', (ws) => {
  console.log('New client connected');

  ws.on('message', (message) => {
    console.log(`Received message => ${message}`);
    // এখান থেকে আপনি ক্লায়েন্টে রিপ্লাই পাঠাতে পারেন
    ws.send('Hello! Message received.');
  });

  ws.on('close', () => {
    console.log('Client has disconnected');
  });
});

console.log('WebSocket server is running on port 8080');

<!DOCTYPE html>
<html>
<head>
  <title>WebSocket Client</title>
</head>
<body>
  <h1>WebSocket Client</h1>
  <script>
    const ws = new WebSocket('ws://localhost:8080');

    ws.onopen = () => {
      console.log('Connected to the server');
      ws.send('Hello Server');
    };

    ws.onmessage = (message) => {
      console.log(`Server says: ${message.data}`);
    };

    ws.onclose = () => {
      console.log('Connection closed');
    };
  </script>
</body>
</html>

const fs = require('fs');
const https = require('https');
const WebSocket = require('ws');

// সার্টিফিকেট এবং কী লোড করা
const server = https.createServer({
  cert: fs.readFileSync('server.crt'),
  key: fs.readFileSync('server.key')
});

// TLS সমর্থিত WebSocket চালানো
const wss = new WebSocket.Server({ server });

wss.on('connection', (ws) => {
  console.log('Client connected over secure WebSocket');

  ws.on('message', (message) => {
    console.log(`Received message => ${message}`);
    ws.send('Secure connection established.');
  });
});

// 443 (HTTPS) পোর্টে সার্ভার চালু
server.listen(443, () => {
  console.log('Server is running on https://localhost');
});

const ws = new WebSocket('wss://localhost');
