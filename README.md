If you want to start the App fresh, with no data, then download the EXE. file and start it up

if you want to start the App with example data showing, please download the "data" file provided and follow the steps below:

- Locate this file location:   C:\Users\<YourName>\The Green Journal\data
- Replace the whole “data” folder with the one provided. 
- Launch the App normally





# The Green Journal

A modern, theme-reactive trading journal built with PySide6 and Python.
Tracks trades, accounts, statistics, equity curves, progress, and funding challenges.

---

## Features

### ✔ Dashboard
- Win rate gauges
- Equity curve (Matplotlib)
- Recent trades list
- PnL calendar
- Auto-refresh via event buses

### ✔ New Trade Page
- Symbol/strategy/direction input
- Auto-colored PnL box
- Screenshot upload + preview
- Ctrl+Enter quick save
- Phase pass / breach detection with sounds

### ✔ Trade History
- Table + Gallery view
- Pagination with Next/Prev
- Filters: dates, accounts, search
- Detailed trade popup

### ✔ Accounts Page
- 1-phase & 2-phase challenges
- Auto phase pass detection
- Breach handling with popup + audio
- Fully theme-reactive cards

### ✔ Settings
- Light/Dark toggle
- Volume slider + test sound
- UI/Popup/Achievement sound toggles
- Export/Import settings
- Reset-to-default popup

---

## Tech Stack

- **Python 3.12**
- **PySide6 (Qt for Python)**  
- **SQLite** database  
- **SQLAlchemy ORM**
- **Matplotlib** (charts)
- **QSoundEffect** (audio engine)
- **PyInstaller** one-file EXE
- Custom:
  - ImageManager
  - SoundBus
  - ToastNotifier
  - BackupManager
  - SettingsManager

---

## Data Location

All data is stored locally at: 
C:\Users<YourName>\TheGreenJournal\

This contains:
- `journal.sqlite3` (database)
- settings
- logs
- backups (optional)

---

## Building the EXE

From the project root:

pyinstaller --onefile --noconsole --name "TheGreenJournal" ^
--icon thegreenjournal/assets/app_icon.ico ^
thegreenjournal/app.py


---

## License
Closed-source. All rights reserved.

