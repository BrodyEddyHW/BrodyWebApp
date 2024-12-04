https://www.figma.com/board/oOBBec5VOeQzFgJINT0s5V/Untitled?node-id=0-1&t=hBJ8j16rslApjzSI-1

# Tech Specification for HW Minimap Game

---

## Overview

The HW Minimap Game is an adaptation of GeoGuessr, designed for Harvard-Westlake students. Players are shown a static image of a campus location and must guess its corresponding position on a minimap. The game provides immediate feedback on the distance between the player's guess and the correct location. Players can submit their scores to a daily leaderboard. The app features a visually appealing UI with Harvard-Westlake branding.

---

## Feature Set

### 1. Start Screen

- **Elements**:
  - Background: White.
  - Logo: Centered Harvard-Westlake Game Logo (static image placeholder if unavailable).
  - "Play Game" Button: Oval-shaped, red with white text, centered.
  - Animation: Button grows slightly on hover.

- **Functionality**:
  - Clicking the "Play Game" button transitions to the gameplay screen.
  - Randomly selects one image from the predefined collection of campus images.

---

### 2. Gameplay Screen

- **Elements**:
  - **Background**:
    - Fills the entire screen with the randomly selected campus photo.
  - **Minimap**:
    - Positioned in the bottom-right corner, expandable when hovered over.
    - Displays a bird’s-eye view map of the HW campus.
    - Has zoom-in/out functionality with user instructions displayed at the bottom-right corner.
    - Marker appears where the user clicks.
  - **Submit Button**:
    - Oval-shaped, red with white text.
    - Positioned at the bottom-center of the screen.

- **Functionality**:
  - Players click on the minimap to select their guess location. 
    - Marker immediately appears where they clicked.
  - The marker on the expanded map stays in the same place when minimap returns to normal size
  - Clicking "Submit Guess" ends the game and transitions to the end screen.

---

### 3. End Screen

- **Elements**:
  - **Distance from correct location**
    - centered
    - format is "x: (horizontal distance)   y: (vertical distance)"
  - **Buttons**:
    - "Play again": bottom-center below the leaderboard, same format as submit button.

- **Functionality**:
  - Displays feedback text: Distance from the correct location, broken into X and Y components.
  - Buttons allow players to:
    1. Restart the game.

---

## Gameplay Features

1. **Randomized Images**:
   - Daily images are rotated from a collection of preloaded campus photos.
   - Each image has associated X and Y coordinates representing the correct location on the minimap.

2. **Map Integration**:
   - The minimap image represents birds-eye view map of the campus.
   - Players interact with the minimap by clicking to drop a marker.

3. **Replayability**:
   - Players can restart the game with a new image by clicking "Play Again."

---

## Visual Design

### Color Palette

- **Primary Colors**:
  - Red (#FF0000): Buttons.
  - Black (#000000): Leaderboard text.
- **Secondary Colors**:
  - White (#FFFFFF): Backgrounds, text on buttons.

---

## Implementation Notes

### HTML

- **Structure**:
  - Three main sections: Start Screen, Game Screen, End Screen.
  - Minimap and its marker are encapsulated within a dedicated `<div>` for styling and event handling.

### CSS

- All screens are styled to fit within a responsive layout.
- Minimap expands on hover for better accessibility and usability.
- Buttons use a consistent hover animation to improve UX.

### JavaScript

- **Randomized Image Selection**:
  - `Math.random()` to select images dynamically.
- **Event Listeners**:
  - Mouse clicks on the minimap register coordinates.
- **Score Calculation**:
  - Distances are from 0 to 1000
  - end screen shows the absolute value of marker position - correct position

---
