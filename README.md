# BIST Trading System Components
# (Borsa Istanbul)
https://www.borsaistanbul.com/files/bistech-itch-protocol-specification.pdf

# Order Book and Network Communication Framework

This repository contains the implementation of an order book system, various data structures, and a basic network communication module. It is designed for use in a trading system, supporting multiple types of order books, parsing, and communication protocols.

## Features

- **Order Book Management**: Implements different types of order books, such as red-black tree, max heap, and linked list-based structures, to handle the order matching process efficiently.
- **ITCH Protocol Support**: Provides basic structures and handling for the ITCH protocol, commonly used in financial data transmission.
- **Hash Tables**: Includes custom hash table implementations for quick data lookups in the order book.
- **IP and Packet Management**: Facilitates low-level IP communication and packet handling, ensuring structured and efficient data transmission.
- **Parsing Engine**: Implements a parser for handling incoming data, useful in extracting and processing messages related to order book updates and trading actions.

## Code Structure

- **Order Book Types**: Supports multiple implementations for managing orders, including:
  - Red-black tree-based order book
  - Max heap-based order book
  - Linked list-based order book
  - Hash-based order book
- **Networking**: Contains modules for managing IP-level communication and handling network packets.
- **ITCH Handling**: Defines structures for ITCH messages, allowing for easy integration with ITCH-compatible systems.
- **Parser**: A robust parsing system for reading incoming data streams, particularly in a trading environment.
- **Utilities**: Helper functions and classes to support the management of different communication and data management operations.

## Dependencies

- **C++17** or later
- **Boost.Asio** (optional, for advanced networking)
- **STL** (for basic data structures)

## Getting Started

### Building the Project

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/repositoryname.git
    cd repositoryname
    ```

2. Ensure that any necessary libraries (e.g., Boost) are installed on your system.

3. Compile the project using your preferred C++ compiler:
    ```bash
    g++ -std=c++17 -o orderbook parser.cpp orderbook.cpp rbt_orderbook.h mheap_orderbook.h ll_orderbook.h hash_orderbook.h -lpthread
    ```

4. Optionally, compile the network communication module:
    ```bash
    g++ -std=c++17 -o network ip.cpp -lpthread
    ```

### Running the Program

- To run the order book system:
    ```bash
    ./orderbook
    ```

- To run the network communication module:
    ```bash
    ./network
    ```

## Contributing

If you encounter any issues or have ideas for improvements, feel free to submit a pull request or open an issue on the repository.

---

This `README.md` provides an overview of the order book system and network communication modules, ensuring clarity and ease of use for users.
