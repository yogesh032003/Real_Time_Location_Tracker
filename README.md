Real-Time Location Sharing with Socket.IO

This project is a real-time location-sharing application built using Express.js and Socket.IO. It allows clients to connect to a server, share their location, and receive location updates from other connected clients.

Features

Real-time Communication: Bidirectional communication using WebSockets.

Location Updates: Broadcasts location updates to all connected clients.

Client Management: Handles client connection and disconnection events.

Getting Started

Follow these instructions to set up and run the project locally.

Prerequisites

Node.js (v12 or higher)

Installation

Clone the repository:

git clone https://github.com/yogesh032003/Real_Time_Location_Tracker
cd Real_Time_Location_Tracker

Install dependencies:

npm install

Running the Application

Start the server:

npm start

Access the application:
Open your browser and navigate to http://localhost:3000 (or the port specified in the PORT environment variable).

Project Structure

real-time-location-sharing/
├── public/           # Static files (HTML, CSS, and client-side JavaScript)
├── server.js         # Main server-side application logic
└── package.json      # Project metadata and dependencies

How It Works

Server Setup:

The server is built using Express.js.

Serves static files from the public directory.

Socket.IO Communication:

Handles real-time WebSocket communication.

Listens for locationUpdate events from clients and broadcasts the location to all connected clients.

Client Lifecycle:

Logs connection and disconnection events.

Example Events

Event: locationUpdate

Emitted by: Clients

Data: Location details (e.g., latitude and longitude)

Server Action: Broadcasts the data to all clients.

Environment Variables

PORT: The port on which the server runs (default: 3000).

License

This project is licensed under the MIT License.

Contributing

Contributions are welcome! Feel free to submit a pull request or open an issue for feature requests or bug reports.


