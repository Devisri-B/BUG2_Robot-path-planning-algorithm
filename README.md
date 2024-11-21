# BUG2 Robot path planning algorithm
it is an implementation of a Bug Algorithm for robot path planning. The Bug2 Algorithm is a basic method used in robotics for navigating a robot from a starting point to a goal while avoiding obstacles in its environment.

## Features

- **Goal-Oriented Navigation**: The algorithm computes a path from the starting point to the goal.
- **Obstacle Handling**: The planner identifies and navigates around obstacles.
- **Visualization**: Includes a graphical representation of the robot's path and obstacles using matplotlib.

## Usage

1. **Initialize the Planner**: Create an instance of the BugPlanner class with the following parameters:
    - start_x, start_y: Starting coordinates of the robot.
    - goal_x, goal_y: Goal coordinates.
    - obs_x, obs_y: Lists of obstacle coordinates.
    - Example:
    ```python planner = BugPlanner(start_x=0, start_y=0, goal_x=10, goal_y=10, obs_x=[3, 6], obs_y=[3, 7])```
2. **Plan the Path**: Use the planner's methods to navigate to the goal while avoiding obstacles. The primary methods include:
    - mov_normal: Direct movement towards the goal.
    - mov_along_obs: Navigation along obstacles.
    - Visualize: Set show_animation = True to display a graphical visualization of the robot's movements and obstacles.
3. **Visualize**: Set show_animation = True to display a graphical visualization of the robot's movements and obstacles.

## Code Structure

### Main Class
  - **BugPlanner**: Implements the Bug Algorithm with methods for movement and obstacle handling.
### Key Methods
  - **mov_normal**: Moves the robot towards the goal in a straight line.
  - **mov_along_obs**: Guides the robot along the edge of an obstacle.
### Variables
  - r_x, r_y: Tracks the robot's position.
  - obs_x, obs_y: Obstacle coordinates.
  - out_x, out_y: Points near obstacles used for navigation.

## Example Output

The algorithm produces a path that avoids obstacles while attempting to reach the goal. The visual output includes:

  - The robot's path.
  - Obstacles and their surrounding clearance zones.
## Future Enhancements

  - Extend support for 3D environments.
  - Incorporate more advanced Bug Algorithm variants.
  - Improve obstacle representation and handling.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your improvements or bug fixes.
  
