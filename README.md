# Quiz Website

## HTML Structure (index.html)
### Head Section
Contains meta tags, title, external CSS (`style.css`), and FontAwesome CDN for icons.

### Body Section
Divided into several main sections:
- **Start Button (`start_btn`)**: Initiates the quiz when clicked.
- **Info Box (`info_box`)**: Provides rules and instructions for the quiz.
- **Quiz Box (`quiz_box`)**: Displays questions, options, and controls.
- **Result Box (`result_box`)**: Displays the quiz result with score and options to replay or quit.

## JavaScript Imports
Includes `questions.js` (for quiz data) and `script.js` (for quiz logic).

## CSS Styling (`style.css`)
### Fonts and General Styling
Defines font styles, background colors, and global styles like box-sizing and margins.

### Positioning and Layout
Uses absolute positioning and transforms to center various boxes (`start_btn`, `info_box`, `quiz_box`, `result_box`) on the screen.

### Animations and Transitions
Utilizes transitions for smooth appearance changes (opacity, transform) and hover effects on buttons.

## JavaScript (`js/script.js`)
### Variable Declarations
Initializes variables for quiz control (start button, info box, quiz box, etc.), timer values, question counters, user score, and more.

### Event Listeners
Handles button clicks (`start_btn`, `exit_btn`, `continue_btn`, `restart_quiz`, `quit_quiz`, `next_btn`) to show/hide quiz elements, start timers, and navigate through questions.

### Functions
- `showQuestions(index)`: Displays questions and options based on the current question index.
- `optionSelected(answer)`: Processes user-selected options, checks correctness, updates score, and manages visual feedback (correct/incorrect).
- `startTimer(time)`: Initializes and updates the countdown timer for each question.
- `startTimerLine(time)`: Animates the timeline progress bar.
- `queCounter(index)`: Updates the question counter display.
- `showResult()`: Displays the final quiz result based on the user's score.

## JavaScript (`js/questions.js`)
### Data Structure
Defines an array `questions` containing objects with properties for each quiz question (`numb`, `question`, `answer`, `options`).

## Explanation of the Project
This quiz application functions by:
- Displaying a start button that opens an info box with quiz instructions.
- Starting the quiz with a timer countdown for each question.
- Presenting questions and options dynamically loaded from `questions.js`.
- Allowing users to select an option, validating correctness, and updating the score.
- Navigating through questions until the end or until the timer runs out.
- Displaying the final score and providing options to replay or quit the quiz.

The CSS styles ensure a visually appealing and responsive layout, while JavaScript handles the quiz logic, timers, and user interactions.

Overall, this project demonstrates the integration of HTML, CSS, and JavaScript to create an interactive quiz application suitable for educational purposes or testing knowledge on specific topics.
