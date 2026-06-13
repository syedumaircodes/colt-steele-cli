# Terminal Commands

The structure of a command and how spaces are used also affect how the shell interprets input. If a user types text directly attached to a command, such as `dateasd`, the shell searches for a single program matching that exact name and will likely return a command not found error. However, inserting a space, as in `date asd`, changes how the shell parses the input. In this case, the shell recognizes `date` as the core command and treats the subsequent text as an argument.

The `date` command displays the current day of the week, month, calendar day, exact time, timezone, and year. This command is highly useful when writing scripts that require precise timestamps to log events, keep in mind that command-line interfaces are generally case sensitive.

## Using Arrow Keys

The left and right arrow keys allow users to navigate the cursor within a line of text in the terminal. This makes it easy to move backward and forward through a command to fix typos, insert new words, or make modifications without deleting the entire line.

The up and down arrow keys perform a different function by letting users cycle through their command history. Pressing the up arrow retrieves previously executed commands, beginning with the most recent, while the down arrow navigates back toward the present.

> [!NOTE]
> The terminal stores a substantial history of commands that can go back several days, though this history is eventually cleared over time.

## Command-line Arguments

Command-line syntax usually follows a basic template, you type the command, add some options, and then hand over the arguments that tell the command to the file or whatever target you want the command to actually act on.

If you are passing multiple arguments, you separate them with spaces. The catch is that the order almost always matters. The command expects its inputs in a very specific sequence, and it will get confused if you mix them up.

The `ncal` command, which displays a calendar. If you want to see July of 1969, you would type `ncal July 1969`. But if you swap them and type `ncal 1969 July`, the command will fail.
