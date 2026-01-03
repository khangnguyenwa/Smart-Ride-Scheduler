# Smart Ride Scheduler

**Smart Ride Scheduler** is a Java console application that simulates a smart ride-booking system similar to Metro Flex. It predicts car arrival times based on customer location and car speed, recommends the optimal car, and automatically reroutes if the selected car is delayed.  

## Features

- Input customer coordinates and minimum wait time.  
- Generate a random fleet of cars with random locations and speeds.  
- Calculate estimated arrival time (ETA) for each car.  
- List all available cars that meet the minimum wait time requirement.  
- Identify the **recommended car** (closest ETA ≥ minimum wait).  
- List cars arriving earlier than the minimum wait time (not recommended).  
- **Smart reroute:** If the recommended car is significantly delayed, automatically suggest a closer car.  

## How It Works

1. The customer enters their X and Y coordinates.  
2. The customer sets the minimum wait time they require for a car.  
3. The system generates a fleet of cars with random positions and speeds.  
4. Each car calculates its ETA to the customer.  
5. Cars with ETA ≥ minimum wait time are listed.  
6. The system recommends the car with the shortest ETA that meets the minimum wait.  
7. Cars arriving too early are displayed but not recommended.  
8. If the recommended car is delayed beyond a threshold, the system reroutes to the nearest available car.  
