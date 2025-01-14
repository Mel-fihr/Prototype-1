# Car Driving Game

## Overview
This repository contains a simple **Car Driving Game** created as part of the Unity "Junior Programmer: Create with Code 1" course. The project focuses on teaching fundamental Unity concepts and basic C# programming through the development of an interactive car simulation game.

## Features
- **Player-controlled car movement:** Use keyboard inputs to drive and steer the car.
- **Physics-based gameplay:** Implemented using Unity's Rigidbody and physics engine.
- **Camera follow system:** A dynamic camera that follows the player's car.
- **Customizable components:** Easily adjust speed, rotation sensitivity, and other parameters in the Unity Inspector.

## Gameplay
- Press **W** or **Up Arrow** to accelerate.
- Press **S** or **Down Arrow** to reverse.
- Use **A/D** or **Left/Right Arrows** to steer the car.

## Technologies Used
- **Unity (Version 2022.3.55f1):** Used to create the game engine and manage the project.
- **C#:** The programming language used for scripting game mechanics.

## Project Structure
```
Car-Driving-Game
├── Assets
│   ├── Scripts
│   │   ├── PlayerController.cs       # Handles car movement and input
│   │   └── FollowPlayer.cs          # Controls the camera's behavior
│   ├── Scenes
│   │   └── MainScene.unity          # Contains the main game environment
│   ├── Prefabs                      # Stores reusable game objects (e.g., the car)
│   ├── Materials                    # Contains visual materials for objects
│   └── Models                       # 3D models used in the game
├── README.md                        # Project documentation
└── .gitignore                       # Specifies files to ignore in version control
```

## Scripts Explanation
### **PlayerController.cs**
- Detects user input and applies it to the car's Rigidbody component to move and steer the vehicle.
- Key variables:
  - `speed`: Controls the forward/backward movement speed.
  - `turnSpeed`: Determines how quickly the car can turn.
  - `horizontalInput`: Captures horizontal input (A/D or Left/Right).
  - `verticalInput`: Captures vertical input (W/S or Up/Down).

### **FollowPlayer.cs**
- Ensures the camera stays focused on the car as it moves.
- Key variables:
  - `offset`: Determines the distance and angle of the camera relative to the car.

## How to Run the Project
1. Clone the repository:
   ```bash
   git clone https://github.com/Mel-fihr/Create-with-Code.git
   ```
2. Open the project in Unity (minimum version 2022.3.55f1).
3. Open the `Prototype 1.unity` file located in the `Assets/Scenes` directory.
4. Press the **Play** button in Unity to test the game.

## How to Customize
- Adjust the **speed** and **turnSpeed** variables in the `PlayerController` script via the Unity Inspector to modify the car's movement.
- Modify the **offset** variable in the `FollowPlayer` script to change the camera's position relative to the car.
- Add obstacles or new elements to the environment for more gameplay variety.

## Challenges and Learnings
This project helped reinforce:
- The basics of Unity's interface and tools.
- Implementing physics-based movement in games.
- Writing clean and reusable C# scripts.
- Managing project files and structure in Unity.

## Contact
For any questions or feedback, please reach out to me at [mel-fihr@student.1337.ma].

