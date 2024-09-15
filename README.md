BIST Trading System Components

(Borsa Istanbul)

Processing Borsa Istanbul orders captured in a pcap file using Wireshark, followed by parsing the data with the ITCH protocol and storing it in four different containers to evaluate the performance of each.
https://www.borsaistanbul.com/files/bistech-itch-protocol-specification.pdf


This project implements various components essential for building and managing an order book system, 
with a focus on financial markets like BIST. It includes multiple data structures, parsers,
and algorithms optimized for high-frequency trading environments.


Features

Red-black tree, hash, and linked list-based order book implementations

Message parsing for financial protocols such as ITCH

Efficient handling of orders and trades

Modular design to support multiple data structures for order management

Usage

The codebase is structured to be easily extended or integrated into larger trading
systems. It supports handling large volumes of financial data in real-time.

