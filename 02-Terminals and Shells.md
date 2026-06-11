# Terminals and shells

People often use the terms terminal and shell interchangeably, but they are actually two different things.  A shell is the software that translates the commands you type into instructions your computer can actually run. It is called a shell because it sits on the outside of the operating system, wrapping around the kernel. A terminal, on the other hand, is just the window where you do the typing. 

Back in the day, terminals were physical boxes with keyboards and screens, wired up to a giant mainframe computer in another room. Today, your terminal is just an app on your desktop that hosts a shell. 

When you type a command and hit enter, the terminal passes that text to the shell. The shell deciphers it, tells the operating system what to do, and sends the result back to the terminal so it can show up on your screen. 
## Command prompt

When you open your terminal, that block of text in the top-left corner is the prompt. What it actually says and what color it is depends entirely on your settings, but it usually lists your username and your computer's network name. 

If you type a valid command, like `clear`, the shell runs it and wipes your screen. If you make a typo or enter a command the shell doesn't recognize, it will spit back an error saying the command was not found. 

Sometimes, the prompt will vanish. This usually means a program is currently running, or a file is still downloading. If you accidentally type an opening quote mark but hit enter before closing it, the prompt will often turn into a simple `>` symbol. This is just the shell waiting for you to finish your thought. 

If you ever get stuck like this and the prompt won't come back, you can usually force your way out and get a clean prompt by pressing `Ctrl + C`. 

---
