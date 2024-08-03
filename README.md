# Keylogger

This Python script implements a simple keylogger using the `pynput` library. The keylogger captures and logs all keystrokes to a file named `keylogger.txt`.

## Features

- Logs all keystrokes, including special keys (e.g., Shift, Ctrl).
- Saves the captured keystrokes to a file (`keylogger.txt`).
- Uses the `pynput` library for capturing keyboard events.

## Requirements

- Python 3.x
- `pynput` library

## Installation

1. Install Python from [python.org](https://www.python.org/).
2. Install the `pynput` library using pip:
    ```sh
    pip install pynput
    ```

## Usage

1. Clone the repository or download the script.
2. Run the script using Python.
3. The script will start logging keystrokes and save them to `keylogger.txt`.

### Running the Script

To run the script, execute the following command in your terminal or command prompt:

```sh
python keylogger.py
```

The script will start listening for keystrokes. Press `Enter` in the terminal to stop the script.

### Example

1. Start the script:
    ```sh
    python keylogger.py
    ```

2. Type some text or press keys.

3. Press `Enter` in the terminal to stop the script.

4. Open `keylogger.txt` to see the logged keystrokes.

## Code Explanation

### Functions

1. **keyPressed(key)**:
    - Called whenever a key is pressed.
    - Prints the key to the console.
    - Appends the key to the `keylogger.txt` file.
    - Handles both regular and special keys.

### Main Execution

1. **if __name__ == "__main__"**:
    - Starts the key listener.
    - Listens for keyboard events and calls `keyPressed` for each key press.
    - Keeps the script running until `Enter` is pressed in the terminal.

### Example Output

1. If you type "Hello123":
    ```txt
    H
    e
    l
    l
    o
    1
    2
    3
    ```

2. If you press special keys like `Shift` or `Ctrl`:
    ```txt
    [Key.shift]
    [Key.ctrl_l]
    ```

## License

This project is licensed under the MIT License.

## Author

Harini

## Contributing

Feel free to fork this repository and submit pull requests. For major changes, please open an issue first to discuss what you would like to change.

## Disclaimer

This script is for educational purposes only. The author is not responsible for any misuse of this script. Always use keyloggers in compliance with local laws and with permission from the device owner.

---

This `README` file provides an overview of the script, its features, usage instructions, and other relevant information for users and contributors.
