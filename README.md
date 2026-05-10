#  Study assistant bot 

A robust Telegram bot built with Python, designed to help students manage their GPA, organize tasks and stay focused using the Pomodoro technique.

##  Live demo
Try the bot here: [t.me/study_assistant_intro_bot]
*(Warning: The bot is active only when the server script is running).*

##  Main features

### 1. GPA calculator
Unlike basic calculators, this module:
* Supports **batch input**: users can paste lists of grades and credits directly.
* Automatically calculates weighted GPA on a 4.0 scale.
* Provides a clean, formatted summary of the semester's performance.

### 2. Pomodoro timer
Engineered using the `threading` library to ensure non-blocking performance:
* Runs focus sessions in the background, allowing users to use other bot features simultaneously.
* Offers presets (25/50 min) and custom time settings.
* Sends automated notifications and updates productivity stats upon completion.

### 3. Interactive to-do manager
Built using an Object-Oriented approach:
* Features dynamic **inline buttons** for instant task completion.
* Includes a built-in "motivation engine" that delivers random encouraging feedback to prevent burnout.

### 4. Analytics & gamification
Tracks user progress over time:
* Monitors total "deep work" hours.
* Logs completed tasks and assigns "Student Ranks" (from beginner to study master).
* Encourages consistency through data-driven feedback.

### 5. Versatile unit converter
A specialized utility for student needs:
* **Conversions:** Weight (Kg/Lbs), Temperature (C/F), Data (GB/MB).
* **Grades:** Instant conversion from percentage scores to letter grades (A, B, C...).

## Technical implementation

* **Framework:** Event-driven architecture using `pyTelegramBotAPI`.
* **State management:** Solved "input-locking" issues by implementing `bot.clear_step_handler_by_chat_id`. This ensures that clicking a menu button immediately resets any pending inputs, providing a seamless User Experience.
* **Concurrency:** Used Python’s `threading` to manage simultaneous countdowns without crashing the main bot loop.
* **UI/UX Design:** A hybrid interface using `ReplyKeyboardMarkup` for navigation and `InlineKeyboardMarkup` for context-specific actions.

## How to run

1. **Install dependencies:**
   ```bash
   pip install pyTelegramBotAPI
2. Configuration:
   Open study_assistant.ipynb and replace the TOKEN variable with your unique API key from @BotFather.
3. Execution
   python study_assistant.ipynb
## The author
**Gissatden Nuradil** at Maqsut Narikbayev university
