# Quest - Habits & Beliefs

Quest is a browser-based habit tracker that blends daily actions with mindset training. Everything lives in `index.html`; there is no build step or server required.

## How the App Works

1. **Forge your mission.** On first launch you pick a weekly rest day (your *Día de Festín*), name a habit with a specific time and place, and optionally write a belief statement that will guide you. This information is saved in `localStorage`.
2. **Daily grid.** A grid of 21 boxes (Quest&nbsp;1) or 60 boxes (Quest&nbsp;2) represents each day of your mission. The box for your rest day shows a grape icon, completed days fill with a golden overlay, and the current day is highlighted.
3. **Daily entry form.** On days that are not your rest day you enter:
   - A belief statement (pre-filled from the previous entry).
   - Evidence supporting that belief. The app cycles through six evidence types such as Memory, Consequence, and Soma (body & mind). Each type has a help dialog with Spanish explanations and examples.
   - A small reward for finishing the habit.
   When you confirm, the entry is saved and confetti celebrates your progress.
4. **Manuals and prompts.** Oracle-style manuals describe Quest&nbsp;1 and Quest&nbsp;2 in detail. After you complete 21 entries you can choose to keep going or start Quest&nbsp;2, which spans 60 days and builds a full routine.
5. **Tools.** The top bar lets you modify your quest, export or import progress as JSON, read the manual again, or reset everything. All state remains in the browser.

## Usage

Open `index.html` in your favorite browser and start your quest. Because all logic and data storage happen client‑side, the app works offline once loaded.

## Contributing

Pull requests are welcome. Please keep code and documentation changes clear and concise.

## Changelog

All notable changes to this project will be documented below.

### [0.1.0] - 2025-06-19
- Initial commit with `index.html` implementing the habit tracking app.

### [0.2.0] - 2025-06-20
- Add README with changelog.
- Improve README with a detailed explanation of how `index.html` works.
- Plan future enhancements such as mobile optimizations, data export/import improvements, and additional quests.
- Fix grid progress to skip days with no entry.
- Resolve bug where completing a day after skipping filled the wrong square.
- Fix rest day showing one day late due to timezone parsing.
- Introduce a Material 3 Expressive theme with updated colors, fonts, and button styles.

### [Unreleased]
- Add "El Primer Paso" manual access from the Oracle icon and Modify Mission menu.
