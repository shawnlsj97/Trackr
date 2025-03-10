# Trackr

Trackr is a **desktop application that helps you to manage tasks**. Trackr is **optimized for users who prefer to work with a Command Line Interface** (CLI) while still having the benefits of a Graphical User Interface (GUI).

<img src="app.png" width="254" height="400" />

If you can type fast, Trackr can help you complete your task management process faster than traditional GUI apps.

### 1. Quick Start
1. Ensure you have Java `11` or above installed in your computer.
2. Download the latest `trackr.jar` [here](https://github.com/shawnlsj97/duke/releases/tag/v1.0).
3. Copy the file to the folder you want to use as the home folder for your list of tasks.
4. Double-click the file to start to app. The GUI should appear shortly.
<img src="launch.png" width="254" height="400" />

5. Type all commands in the command box at the bottom and press "Enter" on your keyboard to execute it.
e.g. typing `help` and pressing "Enter" will show a list of available commands.
    * Some example commands you can try:
        * `list`: lists all tasks
        * `todo 100 pushups`: adds a task to be done called `100 pushups` to the task list
        * `delete 1`: deletes the 1st task shown in the list
        * `exit`: exits the app
        * Refer to the section below for details of available commands in this application

### 2. Features

Words in `UPPER_CASE` are the parameters to be supplied by the user e.g. in `todo TASK_NAME'`, `TASK_NAME` is a parameter which can be used as `todo gym workout`.

#### 2.1 Viewing help: `help`
Displays all available commands in the application.

Format: `help`

#### 2.2 Adding a task to be done: `todo` (alias `t`)
Adds a task to be done with the provided `TASK_NAME` to your list.

Format: `todo TASK_NAME` or `t TASK_NAME`

Examples: 
* `todo 100 pushups`
* `t 100 pushups`
    
    Adds a task to be done with the name `100 pushups` to your list of tasks.

Expected Outcome:

<img src="todo.PNG" width="254" height="108" />

#### 2.3 Adding a deadline: `deadline` (alias `d`)
Adds a deadline with the provided `DEADLINE_NAME` and date and time in the format `DD/MM/YYYY HHMM` to your list.

Format: `deadline DEADLINE_NAME /by DD/MM/YYYY HHMM` or `d DEADLINE_NAME /by DD/MM/YYYY HHMM`

Examples: 
* `deadline math assignment /by 30/11/2019 2359`
* `d math assignment /by 30/11/2019 2359`

    Adds a deadline with the name `math assignment` to be completed by `30/11/2019 2359` to your list.

Expected Outcome:

<img src="deadline.PNG" width="254" height="109" />

#### 2.4 Adding an event to be attended: `event` (alias `e`)
Adds an event with the provided `EVENT_NAME` and date and time in the format `DD/MM/YYYY HHMM` to your list.

Format: `event EVENT_NAME /at DD/MM/YYYY HHMM` or `e EVENT_NAME /at DD/MM/YYYY HHMM`

Examples: 
* `event birthday party /at 28/10/2019 1930`
* `e birthday party /at 28/10/2019 1930`
    
    Adds an event with the name `birthday party` to be attended on `28/10/2019 1930` to your list.

Expected Outcome:

<img src="event.PNG" width="254" height="110" />

#### 2.5 Listing all tasks: `list` (alias `l`)
Shows all tasks in your list.

Format: `list` or `l`

Expected Outcome:

<img src="list.PNG" width="254" height="129" />

#### 2.6 Updating name of task in your list: `update` (alias `u`)
Updates name of specified (using `INDEX`) task in your list to `NEW_TASK_NAME`.

Format: `update INDEX NEW_TASK_NAME` or `u INDEX NEW_TASK_NAME`

Examples: 
* `update 1 50 situps`
* `u 1 50 situps`

    Updates the name of the task in position `1` to `50 situps`.

Expected Outcome:

<img src="update.PNG" width="254" height="112" />

#### 2.7 Retrieving tasks by name: `find` (alias `f`)
Finds tasks whose names contain any of the given `KEYWORD`. You may input multiple keywords.

Format: `find KEYWORD` or `f KEYWORD`

Examples: 
* `find assignment`
* `f assignment`

    Retrieves tasks containing the word `assignment` in their name.

Expected Outcome:

<img src="find.PNG" width="254" height="106" />

#### 2.8 Marking a task as completed: `complete` (alias `c`)
Marks specified (using `INDEX`) task on the list as completed.

Format: `complete INDEX` or `c INDEX`

Examples: 
* `complete 1`
* `c 1`

    Marks the task in position `1` as completed.

Expected Outcome:

<img src="complete.PNG" width="254" height="109" />

#### 2.9 Removing a task: `remove` (alias `r`)
Remove specified task from the list.

Format: `remove INDEX` or `r INDEX`

Examples: 
* `remove 1`
* `r 1`

    Removes the task in position `1` from the list.

Expected Outcome:

<img src="remove.PNG" width="254" height="113" />

#### 2.10 Undoing previous command: `undo`
Undo previous command and revert changes to the list of tasks.

Format: `undo`

Expected Outcome:

<img src="undo.PNG" width="254" height="113" />

#### 2.11 Display input history: `history`
Display all input you made into the application during the current session.

Format: `history`

Expected Outcome:

<img src="history.PNG" width="254" height="148" />

#### 2.12 Exiting the application: `exit`
Exits the program.

Format: `exit`

#### 2.13 Saving data
Task list data is saved in the hard disk automatically after any command that changes the data.
There is no need to save manually.

### 3. FAQ
*Q*: How can I transfer my task list to a new computer?
*A*: Install the app in the other computer and overwrite the empty data file it creates with the file that contains the data of your previous Trackr folder.

### 4. Feedback, Bug Reports

* If you have feedback or bug reports, please post in [shawnlsj97/duke issue tracker](https://github.com/shawnlsj97/duke/issues).
* We welcome pull requests too.

### 5. License
Trackr is [MIT-licensed](https://github.com/shawnlsj97/duke/blob/master/LICENSE).


### 6. Command Summary
* **Add**
    * **Todo**: `todo TASK_NAME`
    * **Deadline**: `deadline DEADLINE_NAME /by DD/MM/YYYY HHMM`
    * **Event**: `event EVENT_NAME /at DD/MM/YYYY HHMM`
* **Update**: `update INDEX NEW_TASK_NAME`
* **List**: `list`
* **Find**: `find KEYWORD`
* **Complete**: `complete INDEX`
* **Remove**: `remove INDEX`
* **Undo**: `undo`
* **History**: `history`
* **Help**: `help`
* **Exit**: `exit`