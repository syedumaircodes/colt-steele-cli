# Terminal Commands

The structure of a command and how spaces are used also affect how the shell interprets input. If a user types text directly attached to a command, such as `dateasd`, the shell searches for a single program matching that exact name and will likely return a command not found error. However, inserting a space, as in `date asd`, changes how the shell parses the input. In this case, the shell recognizes `date` as the core command and treats the subsequent text as an argument.

The `date` command displays the current day of the week, month, calendar day, exact time, timezone, and year. This command is highly useful when writing scripts that require precise timestamps to log events, keep in mind that command-line interfaces are generally case sensitive.

## Using Arrow Keys

The left and right arrow keys allow users to navigate the cursor within a line of text in the terminal. This makes it easy to move backward and forward through a command to fix typos, insert new words, or make modifications without deleting the entire line.

The up and down arrow keys perform a different function by letting users cycle through their command history. Pressing the up arrow retrieves previously executed commands, beginning with the most recent, while the down arrow navigates back toward the present.

> [!NOTE]
> The terminal stores a substantial history of commands that can go back several days, though this history is eventually cleared over time.

## Command-line Arguments

Most command-line interactions follow a consistent formula where a command name is followed by optional options and arguments. Arguments, which are also referred to as parameters or operands, are specific values that users provide for a command to work with or act upon.

When a command accepts multiple arguments, each value must be separated by a space. The order of these arguments is highly important because the system expects them in a specific sequence. For instance, the `ncal` command can accept both a month and a year as arguments, such as `ncal July 1969`. However, reversing this order to `ncal 1969 July` will cause an error because the program is programmed to process the month first and the year second.
