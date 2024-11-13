# Game Overview

The game is a Harvard-Westlake-based adaptation of GeoGuessr. Each day, players are given a photo of a location somewhere on campus, and using a detailed map of the school, they must guess the spot of the location in the photo as accurately as possible. A daily leaderboard tracks scores based on proximity to the actual location and the speed of the guess.

## Theme/Color Scheme

- **Colors:** Red, black, and gold theme (Harvard-Westlake colors)
- **Background:** An aesthetic picture of HW, like the field at sunset
- **Logo:** Game logo centered with a “Play Game” or “Play Now” button below
- **Play Button:** Oval-shaped, centered, red with white text

### Layout

- **Leaderboard:** Left side of the screen, rectangle with rounded corners, black background with white text showing:
  - Format: `placement` `name` `score` `time`
- **Rules List:** Small list on the right side, similar format to the leaderboard

### Gameplay Screen

- **Photo Display:** Once the player clicks “Play Game,” they’re taken to a screen where the daily picture fills the screen. It is static image, so know moving or panning around but the player can zoom in

- **Mini Map:** In the top right corner, expandable on click, with text in the bottom right corner showing how to zoom-in. 
- **Marker:** A marker shows where the player clicks to guess the location
- **Submit Button:** Oval-shaped, red, located at the bottom center, labeled “Submit Guess”
- **Campus Map:** Map is a bird's-eye view of HW upper school campus with white text labels for the different buildings
- **Timer:** Located in the top left corner, format is: `Time: mm:ss`

- submit button and timer stay there when player enters the map
- marker shows on the minimap as well if they player then exits the minimap

### End Screen
- New screen shown after game is complete
- **Leaderboard Display:** Centered on screen, with the player’s new score highlighted
- **Buttons:** Three options below the leaderboard:
  - View picture again
  - Share score
  - Return to main screen

## Typography

- **Primary Font:** Bold or semi-bold Lato
- **Secondary Font:** Regular or light Lato

### Difficulty
- Normal
- Whiteboards only