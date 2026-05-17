# Diet & Sport Wiki Instructions

This file contains the operational rules for automated wiki management.

## 🌍 Language & Setup
- **Initial Setup:** During the first interaction with a new user, you MUST ask for their preferred language (e.g., English, Italian, Spanish).
- **Localization:** Once the language is selected, you must:
    1. Translate the core files (`index.md`, `profile.md`, `Body_Measurements.md`) if they are not already in the target language.
    2. Use the chosen language for all future interactions and file updates.
    3. Store the language preference in the `profile.md` file under a "Settings" or "Preferences" section.

## 📥 Input Types
- **Natural Language (Default):** Process any unstructured text provided by the user (e.g., "I ate an apple", "30min of yoga").
- **Mobile Template (Optional):** Recognize and parse inputs matching the structure of `Templates/Mobile_Input_Prompt.md`. When this format is used:
    1. Extract data from all sections (Diet, Sport, Body).
    2. Process each section using its respective workflow (Dietary, Sports, Profile Management).
    3. You may process multiple updates in a single turn.

## Dietary Workflow
1. **Input:** The user provides meals for the day or a single moment (e.g., "I ate lasagna").
2. **Calculation:** Calculate calories, protein (g), fat (g), carbohydrates (g), and fiber (g) based on reliable average estimates for the indicated portions (or estimated if not specified).
3. **Storage:**
   - Identify the current week (format `YYYY-weekWW`).
   - Look for the file in `Diet/YYYY-weekWW.md`. If it doesn't exist, create it using the template `Templates/Diet_Weekly_Template.md` (replacing `{{date:gggg-WW}}` with the correct week).
   - Add or update the section for the current day (e.g., `## Monday`).
   - Insert data in a structured table or list by meal (Breakfast, Lunch, Dinner, Snacks).
   - Include a daily total of macros and calories.

## Sports Workflow
1. **Input:** The user reports a physical activity (e.g., "30 min of slow running").
2. **Calculation:** Consult `profile.md` for body data and estimate calories burned (MET * weight * time).
3. **Storage:**
   - Look for the file in `Sport/YYYY-weekWW.md`. If it doesn't exist, create it using the template `Templates/Sport_Weekly_Template.md` (replacing `{{date:gggg-WW}}` with the correct week).
   - Add the activity under the corresponding day.
   - Include: Activity type, Duration, Estimated intensity, Calories burned.

## Profile & History Management
- Every time the user updates weight or circumferences in `profile.md`:
    1. Automatically recalculate indicators in the "Calculated Indicators" section of `profile.md`.
    2. Add a new row with the current date in the `Body_Measurements.md` file to track evolution.
- **Exhortation:** At least twice a month (indicatively on the 1st and 15th), if the user hasn't done so, gently remind them to update their body data to keep calculations accurate.

## Index Maintenance
- When creating a new weekly file in `Diet/` or `Sport/`, ensure you update the "Current Week" links in the `index.md` file.

## Monthly Reports
- **Frequency:** At the beginning of each new month, or upon user request.
- **Proactive Check:** At the start of each session in a new month, check if weekly logs exist for the previous month in `Diet/` or `Sport/`. If they exist but the corresponding monthly file is missing in `Diet/Monthly/` or `Sport/Monthly/`, proactively remind the user to generate the monthly report.
- **Procedure:**
    1. Create a new file in `Diet/Monthly/YYYY-MM.md` and `Sport/Monthly/YYYY-MM.md` using the respective templates in `Templates/`.
    2. Consolidate data from the weeks belonging to that month.
    3. Calculate monthly totals and daily averages.
    4. Provide at least 3 qualitative insights based on the data (e.g., "You maintained a constant protein average", "Running volume increased by 10%").
    5. Update links in `index.md` to point to the "Current Month".

## Obsidian Formatting
- Use Obsidian Callouts to highlight important insights.
- Keep files clean and readable.
