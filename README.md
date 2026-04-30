# Real-Time Chat Application (Node.js + WebSockets)

## Overview
A real-time chat application that enables users to communicate instantly using event-driven architecture. The system supports group chats and direct messaging with low-latency message delivery.

## Key Features
- Real-time messaging using WebSockets
- Group chat and one-to-one communication
- Event-driven backend for instant updates
- Responsive UI for cross-device usage

## Tech Stack
- Backend: Node.js
- Frontend: HTML, CSS, JavaScript
- Communication: WebSockets
- Protocol: Matrix.org (for decentralized messaging)

## System Design
The application follows an event-driven architecture:

- Clients establish persistent WebSocket connections with the server
- Messages are sent as events and broadcast to relevant users
- Server handles connection management and message routing
- Ensures low-latency communication by avoiding repeated HTTP requests

## How It Works
1. User connects to server via WebSocket
2. Server registers active connections
3. Messages are emitted as events
4. Server broadcasts messages to target users or groups
5. Clients update UI in real time

## Setup Instructions

```bash
npm install
node server.js
