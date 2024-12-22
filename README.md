# High-Performance Trading and WebSocket Server System

## Overview
This project is a high-performance order execution and management system built to trade on the Deribit Testnet API. It includes a robust WebSocket server for real-time market data streaming, enabling seamless interaction between trading clients and the system.

## Key Features

### **Order Execution and Management**
- **Place Orders:** Submit buy or sell orders with configurable parameters like instrument, price, and amount.
- **Cancel Orders:** Efficiently cancel specific orders by their unique ID.
- **Modify Orders:** Dynamically update existing orders for price and quantity adjustments.
- **Retrieve Open Orders:** Fetch details of all active orders.

### **Market Data Management**
- **Order Book Retrieval:** Access real-time order book data for any trading instrument.
- **View Positions:** Display detailed information on current positions, including size, average price, and mark price.

### **WebSocket Server**
- **Client Connectivity:** Supports multiple client connections via Boost.Asio and Boost.Beast.
- **Dynamic Subscriptions:** Allows clients to subscribe to specific symbols for real-time order book updates.
- **Real-Time Broadcasting:** Continuously streams live updates for subscribed symbols to all connected clients.

## Technology Stack
- **C++**: Core implementation language.
- **Boost.Asio and Boost.Beast**: For WebSocket server functionality.
- **cURL**: For making HTTP requests to the Deribit API.
- **nlohmann/json**: For JSON parsing and manipulation.

## Project Structure
```
project_root/
├── main.cpp          # Entry point for the application.
├── websocket/        # Contains WebSocket server logic.
│   ├── server.h      # Header file for WebSocket server class.
│   └── server.cpp    # Implementation of WebSocket server functions.
```

