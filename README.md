# Customer Delivery Optimization using Reinforcement Learning
## Project Overview
This project focuses on solving the Vehicle Routing Problem (VRP) for customer delivery using Reinforcement Learning (RL). The goal is to optimize delivery routes for vehicles, minimizing total travel distance while meeting customer demands within vehicle capacity constraints.

## Key Features
Reinforcement Learning Approach: Uses the REINFORCE algorithm to optimize delivery routes dynamically.
Custom Environment: Simulates the delivery process with real-world constraints like vehicle capacity and unvisited customer tracking.
Dynamic State Representation: Incorporates the vehicle's current state, load, and customer demands for decision-making.
Scalable Design: Can be adapted to more complex VRP variants, including time windows and multi-depot routing.

## Dataset
The dataset is sourced from an Excel file containing:
Customer Locations (x, y): Specifies customer coordinates.
Depot Locations (x, y): Starting and ending points for vehicles.
Demands: Randomized values representing customer delivery requirements.
Vehicle Capacity: A predefined limit for each vehicle.

## Algorithm Details
Reinforcement Learning (REINFORCE)
Policy Network: A fully connected neural network that predicts probabilities for visiting customers based on the vehicle's current state.
State Representation:
Vehicle's current position (x, y).
Remaining load capacity.
Unvisited customer coordinates and demands.
Action: Choosing the next customer to visit.
Reward: Negative of the travel distance, encouraging shorter routes.
Loss Function: Policy gradient loss with normalized cumulative rewards.

## Results
The RL agent learns to generate efficient routes, reducing travel distance while fulfilling all customer demands.
Visualizations show the optimized routes for vehicles, starting and ending at the depot.

## Future Enhancements
Add time-window constraints for delivery.
Include real-world traffic data for dynamic routing.
Extend to multi-depot routing scenarios.
Experiment with advanced RL algorithms like Proximal Policy Optimization (PPO).
