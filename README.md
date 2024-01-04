# Digital Clock Batch Script

This batch script creates a simple digital clock display along with the current date. It utilizes the Windows command prompt to continuously update the time and date on the screen.

## Usage

1. **Clone the Repository:**
    ```bash
    git clone https://github.com/chhabinath/cmd-clock.git
    ```

2. **Run the Script:**
    - Double-click the `digital_clock.bat` file to launch the digital clock display.
    - Alternatively, run it from the command line by navigating to the folder containing the script and executing `digital_clock.bat`.

3. **Customization:**
    - To adjust the appearance or update intervals, edit the script using a text editor.

## Code Explanation

- `@echo off`: Disables displaying commands in the command prompt.
- `Title digital clock`: Sets the title of the command prompt window to "digital clock."
- `@mode con cols=30 lines=7`: Sets the window size to 30 columns and 7 lines.
- `color 03`: Sets the text and background color to green and blue, respectively.
- `:main` and `goto main`: Label and loop structure to continuously update the time and date.
- `echo Time: %time%` and `echo Date: %date%`: Displays the current time and date.
- `ping -n 2 0.0.0.0>nul`: Pauses for 2 seconds before refreshing the display.
