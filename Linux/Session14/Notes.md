- ### In Virtual box after starting the machine  
Goto view menu -> select aspect ratio dependents on your machine and choose 250% autoscaled for adjusting your screen.  

- **[Ctrl = right side on the keyboard]**  
- **Ctrl + C** = Scaled Mode (Menu Hide/Show)  
- **Ctrl + F** = Fullscreen mode


# Linux Terminal

1.  **Ctrl + C** = Kills the current running process.
2.  **Ctrl + L** = Clears the screen.
3.  **Ctrl + A** = Moves the cursor to the beginning of the line.
4.  **Ctrl + E** = Moves the cursor to the end of the line.
5.  **Ctrl + U** = Deletes the characters from the current cursor position to the beginning of the line.
6.  **Ctrl + K** = Deletes the characters from the current cursor position to the end of the line.
7.  **Ctrl + R** = Search in the history of commands.
8.  **Up Arrow** = Brings previously typed commands.
9.  **Down Arrow** = Navigates back to the current commands.
10. **Ctrl + Left Arrow** = Moves one word to the left of the current cursor position.
11. **Ctrl + Right Arrow** = Moves one word to the right of the current cursor position.
12. **Ctrl+Shift+C**=Copy Text
13. **Ctrl+Shift+V**=Past Text


# Bash command structure
**command [options] [inputs]**

**Options** = Customizing the way command works or tweaking the output.Is a way through which we can pass additional instrcution asking the command to perform the operation.
- `command [option]`
- `-character`
- For every command, options are optional to be passed.
- For a command we can pass multiple options as well:
  - `command -option1 -option2 -option3`
  - `command -option1option2option3`

**Inputs** = Acts as input for the command on which it has to perform the operation.
- Inputs are optional and may not exist for few commands in linux.

--------

# File and Folder

**File** = It is used for storing sequence of set of characters or data on a disk or storage device.  
We always organize and store the data as part of a file so that we can access it collectively/easily.

Open Terminal Window we will be under a default prompt directory called User home.  
`/home/anil/`

**`cd directory/path`** = Change directory  
**`cd ..`** = Moves you to the parent directory.
**pwd**=print working directory

# Linux Commands

**`touch`** is a command used for creating an empty file.

**Syntax:**  
`touch filename` = Creates an empty file in the present working directory.

**`echo`** is used for displaying the text on the terminal.

**Example:**  
`echo "Good Morning"` = It prints "Good Morning" to terminal.

**`cat filename`** = Displays the contents of the file.

**Example** Create an empty file and write content into it

**Create empty file:**  
`touch filename`

**Write content to file:**  
`echo "text" > filename`
