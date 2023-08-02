# Task-Automation-using-Python

This is a simple task automation program built using Python.

This script is designed to automate routine system cleaning tasks ( temporary files ).

In order to schedule the script to run at specific intervals automatically, you will need to use 'Task Scheduler' for Windows, or 'cron' for Linux. Follow these steps:

Windows:
1. Open Task Scheduler by typing "Task Scheduler" in the Windows search bar and selecting the "Task Scheduler" app from the search results.
2. Create a new basic task, provide a name, and set the trigger (e.g., daily, weekly, or at logon).
3. Choose "Start a program" as the action, browse to the Python script file, and set the desired conditions and settings.
4. Review and confirm the task settings to schedule the script to run automatically at the specified intervals.

Linux:
1. Open a terminal window.
2. Enter crontab -e to edit the cron table.
3. Add a new line to the crontab file with the desired schedule and the command to run the Python script. For example:
0 2 * * * /usr/bin/python3 /path/to/your_script.py #runs the script every day at 2:00 AM
4. Save the crontab file and exit the text editor.
