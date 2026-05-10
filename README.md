# 🎓 Study Assistant Bot — All-in-One Academic Toolkit

A robust Telegram bot built with Python, designed to help students manage their GPA, organize tasks, and stay focused using the Pomodoro technique.

## 🔗 Live Demo
Try the bot here: [t.me/YOUR_BOT_USERNAME]
*(Note: The bot is active only when the server script is running).*

---

## 🚀 Key Features

### 1. 🧮 Advanced GPA Calculator
Unlike basic calculators, this module:
* Supports **batch input**: users can paste lists of grades and credits directly.
* Automatically calculates weighted GPA on a 4.0 scale.
* Provides a clean, formatted summary of the semester's performance.

### 2. ⏰ Multithreaded Pomodoro Timer
Engineered using the `threading` library to ensure non-blocking performance:
* Runs focus sessions in the background, allowing users to use other bot features simultaneously.
* Offers presets (25/50 min) and custom time settings.
* Sends automated notifications and updates productivity stats upon completion.

### 3. 📝 Interactive To-Do Manager (OOP Based)
Built using an Object-Oriented approach:
* Features dynamic **Inline Buttons** for instant task completion.
* Includes a built-in "Motivation Engine" that delivers random encouraging feedback to prevent burnout.

### 4. 📈 Analytics & Gamification (Study Stats)
Tracks user progress over time:
* Monitors total "Deep Work" hours.
* Logs completed tasks and assigns "Student Ranks" (from Beginner to Study Master).
* Encourages consistency through data-driven feedback.

### 5. 🔢 Versatile Unit Converter
A specialized utility for student needs:
* **Conversions:** Weight (Kg/Lbs), Temperature (C/F), Data (GB/MB).
* **Grades:** Instant conversion from percentage scores to Letter Grades (A, B, C...).

---

## 🛠 Technical Implementation

* **Framework:** Event-driven architecture using `pyTelegramBotAPI`.
* **State Management:** Solved "input-locking" issues by implementing `bot.clear_step_handler_by_chat_id`. This ensures that clicking a menu button immediately resets any pending inputs, providing a seamless User Experience (UX).
* **Concurrency:** Used Python’s `threading` to manage simultaneous countdowns without crashing the main bot loop.
* **UI/UX Design:** A hybrid interface using `ReplyKeyboardMarkup` for navigation and `InlineKeyboardMarkup` for context-specific actions.

---

## 📦 How to Run

1. **Install Dependencies:**
   ```bash
   pip install pyTelegramBotAPI
