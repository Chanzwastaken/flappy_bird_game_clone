# Flappy Bird Game Clone
![image](https://github.com/user-attachments/assets/d68a7c35-0586-49bb-ac14-808ab48b94cb)


## Overview
Flappy Bird is an arcade-style game where the player controls the bird, Faby, which moves persistently to the right. The player must navigate Faby through pairs of pipes with equally sized gaps placed at random heights. Faby automatically descends and only ascends when the player taps the touchscreen. Each successful pass through a pair of pipes awards the player one point. Colliding with a pipe or the ground ends the gameplay.

## Features
- **Game State Management**: Uses Flame and Flutter for efficient game state management.
- **UI and Logic Separation**: Ensures a clean separation of user interface and game logic.
- **Cross-Platform Support**: Play Flappy Bird on Android, iOS, web, and desktop platforms.

## Technologies Used
- **Flutter**: For building a high-performance, cross-platform application.
- **Dart**: The programming language used for Flutter development.
- **Flame Engine**: Game engine used for game logic and rendering.
- **Visual Studio Code**: The IDE used for development.
- **Git**: For version control and collaboration.

## Getting Started
Follow these instructions to get a copy of the project up and running on your local machine.

### Prerequisites
- Flutter SDK: [Install Flutter](https://flutter.dev/docs/get-started/install)
- Dart SDK: Included with Flutter

### Installation
1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/flappy-bird-game-clone.git
   cd flappy-bird-game-clone
   ```

2. **Install dependencies:**
   ```bash
   flutter pub get
   ```

3. **Set up Firebase:**
   - Follow the Firebase setup instructions for Flutter [here](https://firebase.flutter.dev/docs/overview/).

4. **Run the application:**
   ```bash
   flutter run
   ```

## State Management Techniques

### Overlay Management
- Uses Flame's `GameWidget` overlays to switch between different game states.
- Overlays are added or removed to transition between the main menu, gameplay, and game over screens.

### Game Loop and Updates
- The `update` method in `FlappyBirdGame` manages the game state by updating the bird's position, score, and checking for collisions.
- The `onTap` method triggers the bird's flight, demonstrating how user input is handled to change the game state.

### Component State
- The bird's state (position, movement, and score) is managed within the `Bird` component.
- The `gameOver` method in the `Bird` component changes the game state to "game over" and pauses the game engine.

### Flutter Widgets
- The main menu and game over screens are managed using Flutter widgets, allowing for a clean separation of UI and game logic.
- The `onRestart` method in the `GameOverScreen` widget resets the bird's state and resumes the game.

## Contributing
We welcome contributions to improve Flappy Bird! Here’s how you can help:
- Report bugs and request features via GitHub Issues.
- Fork the repository, create a new branch, and submit a pull request with your changes.
- Write tests for new features and bug fixes.

## Demo
![image](https://github.com/user-attachments/assets/efd11fac-1841-46e0-8f07-4b6988c2eb05)


## Reference
- [Flame Engine Documentation](https://docs.flame-engine.org/latest/)
- [Flutter Documentation](https://docs.flutter.dev/)
- [YouTube Tutorial](https://www.youtube.com/watch?v=zcs8qRBRz7w)

## Author
M. Chandra Agoeng P - 41522010248
