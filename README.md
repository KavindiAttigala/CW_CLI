
Project Overview

The Ticketing System is a multi-threaded application designed to simulate ticket transactions. Vendors can add tickets to a shared pool, while customers purchase tickets at specified intervals. The system ensures that the total number of tickets does not exceed the defined maximum capacity.

Key Features:
User-configurable settings saved to a JSON file.
Vendors can add tickets to the pool.
Customers can purchase tickets from the pool.
Logs and saves all transactions (additions and purchases) in a JSON file.
Supports concurrent operations by simulating multiple vendors and customers using threads.
Features

Simulation Control: Start and stop the simulation via a command-line interface.
Vendor Management: Vendors add tickets to the pool at specified intervals.
Customer Management: Customers purchase tickets at specified intervals.
Transaction Logging: All ticket transactions are recorded and stored in JSON files for review.
Technologies Used

Java SDK 21: The system is built using Java SDK version 21.
Google Gson Library: Used for JSON serialization and deserialization, enabling efficient management of configuration and transaction data. The Gson JAR file is included in the project.
Setup Instructions

  
Usage

The system begins by prompting the user to decide whether to load the previous configuration.

If the user selects Yes, the system reads the configurations from the configuration.json file, retrieves the settings, and displays a menu to start the simulation.
If the user selects No, the system prompts for four new configurations:
Initial ticket count.
Ticket release rate (e.g., 10 tickets at a time).
Customer purchase rate (e.g., 5 tickets at a time).
Maximum ticket capacity.
Once the configurations are entered, the system offers a menu to initiate the simulation. During the simulation:

Vendors and customers operate concurrently, adding and purchasing tickets.
The user can terminate the simulation at any time by entering an exit code.
After the simulation ends, all transactions are saved in a transaction.json file for record-keeping.
