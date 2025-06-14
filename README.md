# Pomodoro Timer 🍅

A simple and effective Pomodoro Timer application built with Python's Tkinter library to help boost your productivity using the Pomodoro Technique.

## What is the Pomodoro Technique?

The Pomodoro Technique is a time management method that uses a timer to break work into intervals, traditionally 25 minutes in length, separated by short breaks. This technique helps improve focus and productivity while preventing burnout.

## Features

- **25-minute work sessions** followed by breaks
- **5-minute short breaks** after each work session
- **20-minute long break** after every 4 work sessions (8th rep)
- **Visual timer display** with a tomato-themed interface
- **Progress tracking** with checkmarks for completed work sessions
- **Start/Reset functionality** for full timer control
- **Color-coded labels** to distinguish between work and break periods

## Screenshots

The application features a clean, minimalist interface with:
- A tomato image as the central timer display
- Large, easy-to-read countdown timer
- Color-coded status labels (Green for work, Pink/Red for breaks)
- Simple start and reset buttons
- Progress checkmarks below the timer
- ![image](https://github.com/user-attachments/assets/5fee79d5-f3b7-4802-90e0-0f7933b92273)
- ![image](https://github.com/user-attachments/assets/26d5021b-fae3-463f-a48a-4b9993da8f62)



## Requirements

- Python 3.x
- Tkinter (usually comes pre-installed with Python)
- `tomato.png` image file in the same directory as the script

## Installation

1. Clone this repository:
```bash
git clone https://github.com/yourusername/pomodoro-timer.git
cd pomodoro-timer
```

2. Ensure you have the `tomato.png` file in the same directory as the Python script.

3. Run the application:
```bash
python pomodoro_timer.py
```

## Usage

1. **Start Timer**: Click the "Start" button to begin your first 25-minute work session
2. **Work Session**: Focus on your task while the timer counts down
3. **Break Time**: When the work session ends, take your break as indicated
4. **Track Progress**: Checkmarks appear below the timer for each completed work session
5. **Reset**: Click "Reset" at any time to stop and reset the timer

## Timer Flow

- **Reps 1, 3, 5, 7**: 25-minute work sessions (Green label)
- **Reps 2, 4, 6**: 5-minute short breaks (Pink label)  
- **Rep 8**: 20-minute long break (Red label)
- Pattern repeats after rep 8

## Customization

You can easily customize the timer durations by modifying these constants in the code:

```python
WORK_MIN = 25          # Work session duration
SHORT_BREAK_MIN = 5    # Short break duration  
LONG_BREAK_MIN = 20    # Long break duration
```

You can also customize the colors by changing these hex values:
```python
PINK = "#e2979c"
RED = "#e7305b" 
GREEN = "#9bdeac"
YELLOW = "#f7f5dd"
```

## File Structure

```
pomodoro-timer/
│
├── pomodoro_timer.py    # Main application file
├── tomato.png          # Tomato image for the timer display
└── README.md           # This file
```

## Known Issues

- The code contains a syntax error on line 52: `for * in range(work*session):` should be corrected to `for _ in range(work_session):`
- There's an unused import: `from pip._internal.network import session` can be removed

## Contributing

Feel free to fork this project and submit pull requests for any improvements. Some ideas for enhancements:

- Add sound notifications when sessions end
- Save session statistics 
- Add settings panel for custom durations
- Implement keyboard shortcuts
- Add different timer themes



## Acknowledgments

- Inspired by the Pomodoro Technique developed by Francesco Cirillo
- Built with Python's Tkinter for cross-platform compatibility

---

**Happy productivity! 🍅⏱️**
