# HW Minimap Game

The HW Minimap Game is a web-based game inspired by GeoGuessr, tailored for Harvard-Westlake students. Players guess the location of campus landmarks on a minimap and receive feedback on their accuracy.

## Setup Instructions

1. Clone the Repository:  
`git clone <repository-url>`  
`cd <repository-folder>`

2. Install Firebase CLI:  
If you don't already have Firebase CLI installed, install it with npm:  
`npm install -g firebase-tools`

3. Log in to Firebase:  
Log in to your Firebase account:  
`firebase login`

4. Initialize Firebase Hosting:  
Run this command in the project directory:  
`firebase init`  
Select "Hosting" during the setup process and choose the current directory when prompted.

5. Run the Application Locally:  
Start a local server with Firebase:  
`firebase serve`  
Alternatively, use the Live Server extension in VS Code. Install the extension, right click on `index.html`, and click "Open with Live Server" which should be the top option in the dropdown.

6. Open in Browser:  
Access the app at `http://localhost:5000` when using Firebase, or at the generated Live Server URL.

## Key Parts of the Code

### Main Files
- `index.html`: Contains the structure of the website with three main sections: Start Screen (includes the "Play Game" button), Game Screen (displays the game interface with a minimap and gameplay elements), and End Screen (shows results and provides the option to play again).
- `minimap.css`: Provides styling for the start, game, and end screens, including hover animations, button designs, and responsive layouts.
- Inline JavaScript: Handles all game logic, including:
  - Randomly selecting a game image from the collection.
  - Capturing the user's marker location on the minimap.
  - Calculating the distance between the guess and the correct location.

### Key Functions
1. `startGame()`: Hides the start screen, displays the game screen, randomly selects an image, and updates the game screen.
2. `submitLocation()`: Handles the submission of the player's guess, calculates the distance between the guessed location and the correct location, and displays the results on the end screen.
3. `playAgain()`: Resets the game state and restarts with a new randomly selected image.
4. `addImage(x, y)`: Saves the player's click position on the minimap.
5. Event Listener for the Minimap: Registers the player's click and updates the marker's position dynamically.

## Special Instructions & Tools
- **Firebase**: This project uses Firebase Hosting for deployment. Follow the setup instructions above to initialize and serve the project locally or deploy it to the web.
- **Live Server**: During development, the Live Server extension in VS Code was used for real-time previewing.

## Running the Project
Ensure the Firebase CLI is set up as described above. Start the local server with:  
`firebase serve`  
Open your browser and navigate to the provided local URL (e.g., `http://localhost:5000`). Alternatively, use the Live Server extension by opening `index.html` in VS Code and starting the server.

Enjoy playing the HW Minimap Game!
