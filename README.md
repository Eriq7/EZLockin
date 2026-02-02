# EZLockIn (Immersive Study Timer)

A desktop study companion designed to fight **timer anxiety**.  
EZLockIn keeps you focused using two game-inspired mechanics: **randomness** and **rewards**.

---

## Origin & Philosophy

### Why do games keep people playing, but studying feels hard to sustain?

Games stay addictive because they repeatedly trigger two simple mechanisms:

| Game Mechanic | What it does to your brain | How **EZLockIn** uses it |
|---|---|---|
| 🎲 **Randomness** | Keeps you curious because you don’t know what happens next | Focus sessions are **randomized** (e.g., 3m, 5m, 3m15s) |
| 🎁 **Rewards** | Gives small “wins” that motivate you to repeat the loop | Every session ends with a **10-second reward break** |

✅ Result: studying becomes a lightweight **game loop** — less pressure, more momentum.

---

## Core Features

* 🎲 **Random Focus Cycles**: Randomly generates focus durations within a configurable range.
* ☕️ **Smart Break System**: Automatically switches between short breaks and long breaks.
* 📊 **Study Logging**: Logs each completed session to `study_log.csv` for review and analysis.
* 🎨 **Highly Configurable**: Customize timings, sounds, and more using `config.json`.

---

## Quick Start (Recommended)

---

## Usage Guide

* **Move**: Drag the window.
* **Right-click Menu**: Right-click the window to access all features.

#### Right-click Menu Options

| Feature | Description |
| :--- | :--- |
| **Status Info** | Shows current timer state and estimated time until a long break. |
| **▶️ Start / Resume** | Start the timer or resume from pause. |
| **⏸️ Pause** | Pause the current timer. |
| **✅ Always on Top** | Keep the window above other windows. |
| **💧 Opacity** | Adjust the window transparency. |
| **🔄 Reset** | **Reset Current Cycle**: Stops the current cycle and prepares a new one.<br>**Clear All Statistics**: Clears total accumulated focus time (**with confirmation**). |
| **📂 Open Log Folder** | Opens the program folder to view logs and configuration files. |
| **❌ Quit** | Saves data and safely exits the app. |

---

## Custom Configuration (`config.json`)

On first launch, EZLockIn automatically creates a `config.json` file.  
Edit it with any text editor, then restart the app to apply changes.

(Partial parameter reference)

| Parameter | Description |
| :--- | :--- |
| `study_time_min` | Minimum focus duration per round (seconds). |
| `study_time_max` | Maximum focus duration per round (seconds). |
| `long_break_threshold` | Total accumulated focus time required to trigger a long break (seconds). |

---

## For Developers

If you want to run from source, follow these steps.

#### 1. Requirements

* Install [Python](https://www.python.org/) (3.8+ recommended)
* Clone this repo: `git clone https://github.com/Eriq7/EZLockIn.git`
* Enter the project folder: `cd EZLockIn`

#### 2. Install Dependencies

This project uses `requirements.txt` to manage dependencies.

```bash
pip install -r requirements.txt
