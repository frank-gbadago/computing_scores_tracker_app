# Computing Scores Tracker

A simple, browser-based app to record and manage student computing scores. Works offline with localStorage and supports manual backup/sync via Google Drive.

## Features

- **Student Management**: Add, edit, and delete students organized by class (Basic 1-9)
- **Academic Year & Term Support**: Track scores across multiple years and terms (3 terms per year)
- **Score Recording**: Enter Exercise 1 and Exercise 2 scores for each week (1-13)
- **Reports**: View scores by class with statistics (average, highest, lowest)
- **Student Promotion**: Move students between classes when a new academic year begins
- **Export/Import**: Backup and restore data using JSON files (for Google Drive sync)
- **Offline Support**: All data stored locally in your browser

## How to Use

### Option 1: Open Directly
1. Download the `computing-scores.html` file
2. Double-click to open in your browser
3. Start adding students and recording scores

### Option 2: Host on GitHub Pages (Free)
1. Create a new GitHub repository
2. Upload the file and rename it to `index.html`
3. Go to Settings > Pages > Enable GitHub Pages
4. Access your app at `https://yourusername.github.io/repository-name`

## Syncing Between Devices (Google Drive)

Since data is stored locally in each browser, use the Export/Import feature to sync between devices.

### Workflow

| Location | When Done | When Starting |
|----------|-----------|---------------|
| School | Export → Upload to Google Drive | Download from Drive → Import |
| Home | Export → Upload to Google Drive | Download from Drive → Import |

### Export Data
1. Click the **Export** button (blue)
2. A JSON file downloads to your computer
3. Upload this file to Google Drive

### Import Data
1. Download your backup file from Google Drive
2. Click the **Import** button (gray)
3. Select the JSON file
4. Confirm to replace current data

**Important**: Always export before switching devices, or you may lose new entries.

## Data Structure

- **Students**: Stored by academic year and class
- **Scores**: Stored by academic year, term, student ID, and week
- **Promotion**: Students can be moved to new classes while preserving their score history

## Storage

Data is saved in your browser's localStorage under the key `computing_scores_v2`. Clearing browser data will delete your records, so remember to export backups regularly.

## License

Free to use and modify for personal or educational purposes.
