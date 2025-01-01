# Park-Restroom-Planning
This project solves a problem of optimal restroom placement in a park using search algorithms, developed as part of a programming assignment in the NCCU's Introduction to AI course. It demonstrates the implementation of heuristic search techniques like hill-climbing and random-restart hill climbing.

## Features

- **Grid-Based Park Representation**:
  - Park is modeled as an \( n \times m \) grid.
  - Playgrounds and restrooms are positioned on specific grid cells.
- **Optimization Objective**:
  - Minimize the total Manhattan distance between playgrounds and the nearest restroom.
- **Algorithms Implemented**:
  - Hill-Climbing Search.
  - Random-Restart Hill-Climbing Search.

## How It Works

1. **Input**:
   - The grid size (\( n, m \)), playground positions, initial restroom positions, and number of restrooms.
   - Example input format:
     ```
     1
     4,4
     4|0,0|2,0|2,2|3,2
     1
     10
     ```

2. **Algorithm**:
   - Hill-climbing: Iteratively improves the restroom placement by moving to a neighboring position with a lower cost.
   - Random-restart: Performs multiple hill-climbing runs with different starting points to avoid local minima.

3. **Output**:
   - A dictionary containing:
     - Initial cost.
     - Best (minimal) cost.
     - Final restroom locations.

   Example:
   ```json
   {
       "ini_cost": 15,
       "best_cost": 9,
       "locations": [[2,1]]
   }
   ```

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/YourUsername/Park＿Restroom＿Planning.git
   cd Park＿Restroom＿Planning/src
   ```

1. Clone the repository:
   ```bash
   git clone https://github.com/YourUsername/ParkRestroomPlanning.git
   cd ParkRestroomPlanning
   ```

## Tasks Implemented

- **Task 0**: Single restroom optimization using hill-climbing and random-restart hill climbing.
- **Task 1**: Multi-restroom optimization.
- **Task 2 & 3**: Online and hidden test cases for random-restart hill climbing.



## Design Highlights

- **Manhattan Distance Calculation**:
  - Efficient computation of distances between playgrounds and restrooms.
- **Search Techniques**:
  - Local optimization with hill climbing.
  - Enhanced global optimization with random restarts.




