# Delhi Metro Route Planner

Delhi Metro Route Planner is a command-line application that calculates the shortest route between stations on the Delhi Metro network using **Dijkstra's algorithm**. Built in **C++**, it supports finding paths with an optional intermediate station, displays **line color changes** (e.g., Yellow to Blue at Rajiv Chowk), and provides **travel details** such as distance, time, fare, and number of stations. The CLI is enhanced with **metro-line themed color-coded outputs** for an engaging user experience.

---

## Features

- **Shortest Path Calculation**: Implements **Dijkstra's algorithm** to find the optimal route between two Delhi Metro stations, with support for an intermediate stop.
- **Line Color Changes**: Detects and displays metro **line transitions** (e.g., Yellow Line to Blue Line, Aqua Line to Blue Line ) along the route.
- **Travel Details**: Outputs estimated **distance (in km), travel time (in minutes), fare (in INR), and number of stations**.
- **Metro-Themed CLI**: Features **color-coded station names** based on metro lines.
- **File-Based Data**: Reads **station names, line colors, and connectivity** from text files (`stationnames.txt`, `colorcodes.txt`, `nodes.txt`).
- **Interactive Menu**: Offers options to **find a route or exit**, with a smooth transition between screens.

---

## Prerequisites

- **C++ Compiler**: GCC (e.g., **MinGW for Windows**) or any **C++11-compatible** compiler.
- **Operating System**: Tested on **Windows** (uses `windows.h` for console manipulation).
- **Required Text Files**: Ensure the following files are in the project directory:
  - `nodes.txt` (List of station names)
  - `metro_line.txt` (Metro line colors)
  - `edge_info.txt` (Graph representation of the metro network)

---

## Installation & Usage

1. **Clone the repository**:
   ```sh
   git clone https://gitingest.com/sheisstarwithoutmoon/delhi-metro-route-planner.git
   cd delhi-metro-route-planner
   ```

2. **Compile the C++ program**:
   ```sh
   g++ main.cpp -o metro
   ```

3. **Run the program**:
   ```sh
   ./metro  # For Linux/macOS
   metro    # For Windows
   ```

