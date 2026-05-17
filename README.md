# 🥗 Diet & Sport Tracking Wiki (Obsidian + AI)

Welcome to this personal Wiki project for tracking diet and physical activity, designed to work symbiotically with **Obsidian** and an AI assistant (like **Gemini CLI**).

This repository provides a ready-to-use structure for anyone who wants to monitor their health intelligently, automating nutritional calculations and body progress tracking.

## 🚀 Key Features

- **Automated Food Log:** You write what you eat, the AI calculates calories and macros (protein, fat, carbs, fiber) and fills in the weekly files.
- **Sports Tracking:** Calculation of calories burned based on your anthropometric data (MET).
- **Body Evolution:** A system to track weight and circumferences over time with automatic calculation of BMR, TDEE, and Body Fat.
- **Centralized Dashboard:** An `index.md` file that acts as a control center to quickly navigate between logs and progress.
- **Intelligent Reminders:** Integrated instructions to prompt bi-monthly updates of body data.

## ⚠️ Privacy & Security

**IMPORTANT:** If you decide to fork this repository or upload your version to GitHub, **do not publish your personal data!**

Files like `profile.md`, `Body_Measurements.md`, and the contents of the `Diet/` and `Sport/` folders will contain sensitive information about your health and habits.
- Make sure to add these files to your `.gitignore` if you intend to keep the repository public.
- Use this repository as a private or local **template** for your security.

## 📁 Repository Structure

- `Diet/`: Folder for weekly food logs.
    - `Monthly/`: Consolidated monthly reports and insights.
- `Sport/`: Folder for weekly workout logs.
    - `Monthly/`: Monthly performance summaries.
- `Templates/`: Contains templates for quickly creating new logs and the dashboard.
- `profile.md`: Your current body "database".
- `Body_Measurements.md`: Historical table of physical evolution.
- `GEMINI.md`: The instruction file (System Prompt) that guides the AI in managing the wiki.
- `SETUP.md`: Technical configuration guide.

## 🛠 How to Use It

1. **Clone or download** this repository as a new Obsidian vault.
2. **Setup your AI assistant:** Ensure your assistant reads the `GEMINI.md` file.
3. **Run Setup:** During the first interaction, the AI will ask for your preferred language and help you initialize your profile.
4. **Start logging:** Write to your assistant: *"Today for lunch I had 100g of tomato pasta and a chicken breast"* and watch the wiki update itself!

## 📱 Mobile Workflow (On-the-go)

Since Gemini CLI is best used from a terminal, you can log your activities on-the-go using your phone:
1. **Copy the Template:** Copy the content of `Templates/Mobile_Input_Prompt.md` into your favorite mobile notes app (e.g., Apple Notes, Google Keep).
2. **Fill it out:** During the day, jot down what you eat and your physical activity.
3. **Sync:** In the evening, paste the entire note into your Gemini CLI terminal. The AI will automatically parse the data and update all relevant logs at once.

## 🤝 Contributing
This is an open project! If you have suggestions to improve the calculation formulas or the file structure, feel free to open an Issue or a Pull Request.

---
*Created with ❤️ for health and productivity.*
