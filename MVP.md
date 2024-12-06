# MVP: HW Minimap Game

---

## **Current Status**

The HW Minimap Game is operational with the following features fully implemented:

### **Completed Features**

1. **Start Screen**:

   - Displays a "Play Game" button with hover animations.
   - Transitions to the gameplay screen on click.
   - Randomly selects one image from the image collection.

2. **Gameplay Screen**:

   - Displays the selected campus photo as the background.
   - Includes a minimap positioned in the bottom-right corner that expands on hover.
   - Allows players to click on the minimap to select a location.
   - Dynamically displays a marker at the clicked location.
   - Includes a submit button for finalizing the guess.

3. **End Screen**:

   - Displays feedback on the distance (X and Y) between the player's guess and the correct location.
   - Includes a "Play Again" button to restart the game with a new image.

4. **Randomized Image Selection**:

   - Images are selected randomly from a predefined collection.
   - Each image has associated X and Y coordinates for scoring.

5. **Score Calculation**:

   - Calculates the X and Y distances between the player's guess and the correct location.

6. **Replayability**:
   - Players can replay the game by clicking "Play Again."
   - Resets the marker and generates a new random image.

---

## **Next Steps**

### **1. Leaderboard Implementation**

- **Objective**: Add a leaderboard to display top scores and times for the day.
- **Details**:
  - Include player rank, name, score (distance), and time.
  - Highlight the current player's score.
  - figure out how score should be calculated
- **Timeline**: 1-2 days.

### **2. Map Enhancements**

- **Objective**: Improve the usability of the minimap.
- **Details**:
  - Add zoom-in/out controls.
  - Update map and add labels.
  - Extra step could be allowing players to see a floor plan of the building they click on
- **Timeline**: 2 days.

### **3. Improved Aesthetics**

- **Objective**: Enhance the visual appeal to align with Harvard-Westlake branding.
- **Details**:
  - Replace placeholders with an actual logo.
  - Update the start screen background to an HW-themed image (e.g., field at sunset).
  - choose better font
  - generally improve the look of the game
- **Timeline**: 1-2 days.

### **5. Expand Image Collection**

- **Objective**: Add more campus images for variety and daily gameplay.
- **Details**:
  - Add at least 5 additional images for the time being (we will need to add more later).
  - Each image needs predefined X and Y coordinates for the correct location.
- **Timeline**: 1 day.

### **6. Daily Challenges**

- **Objective**: Make it a daily game.
- **Details**:
  - Sync the displayed image across all players based on the current date.
  - Implement a reset at midnight for the next day’s challenge.
  - reset daily leaderboard
  - block players from getting multiple tries on the same day
- **Timeline**: 2 days.

---

## **Future Development Goals**

1. **Social Sharing**:

   - Allow players to share their scores directly via a social media mockup.
   - Add a "Share Score" button to the end screen.

2. **Mobile Optimization**:

   - Ensure the game is fully responsive and playable on mobile devices.
   - Adapt the minimap and marker functionality for touchscreens.

3. **Multiplayer Mode**:
   - Implement a real-time multiplayer mode where players compete to guess locations the fastest.

---

## **Proposed Timeline**

| Task                       | Estimated Time | Completion Date |
| -------------------------- | -------------- | --------------- |
| Leaderboard Implementation | 1-2 days       | TBD             |
| Timer Functionality        | 1 day          | TBD             |
| Map Enhancements           | 2 days         | TBD             |
| Improved Aesthetics        | 1-2 days       | TBD             |
| Expand Image Collection    | 1 day          | TBD             |
| Daily Challenges           | 2 days         | TBD             |
| Social Sharing             | Future         | TBD             |
| Mobile Optimization        | Future         | TBD             |
| Multiplayer Mode           | Future         | TBD             |

---

## **Summary**

The HW Minimap Game is fully functional in its current state, meeting the requirements of an MVP. The next steps focus on enhancing the user experience, adding replayability features (leaderboard, timer), and improving aesthetic alignment with Harvard-Westlake branding. The outlined timeline ensures a clear, actionable path forward for future development.
