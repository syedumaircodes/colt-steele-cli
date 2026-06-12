# Command-line options

Options (often called flags) are tools you use to change how a command behaves. They usually start with a single dash so the computer knows they are options, not arguments.

Keep in mind that options are strictly case-sensitive. In the terminal, lowercase and uppercase letters are completely different characters. A lowercase option might do one thing, while its uppercase counterpart does something else entirely.

Take the calendar command, `ncal`. If you run it by itself, you get a standard calendar. If you add the `-h` option, it turns off the highlighting on today’s date. Add `-j` and it switches to Julian days (numbering days from 1 to 365 starting January 1st). The `-M` option starts the week on Monday instead of Sunday, and `-3` shows you three months at once. Think of options as custom toggles for your commands.

## Multiple options

If you need to use more than one option at a time, you can write them out separately with spaces in between. To show three months of the calendar without highlighting today’s date, you can run:

```bash
ncal -3 -h
ncal -3h
```

Both methods do the exact same thing. This shortcut is a lifesaver when you are stacking a lot of options.

## Long form options

While most options are single letters, some have long-form names written out as full words. These require a double dash instead of a single one.

The double dash tells the shell to read the whole word as one option, rather than trying to parse it as a bunch of single-letter flags mashed together. If you typed `-universal`, the terminal would think you were trying to run options `-u`, `-n`, `-i`, `-v`, and so on, which will usually blow up in an error.

Many commands support both styles. For example, `date -u` and `date --universal` both show the time in UTC. On the `sort` command, `-r` and `--reverse` reverse your alphabetical sorting, while `-u` and `--unique` filter out duplicate lines.

> [!NOTE]
> You cannot chain long-form options together under a single prefix. You have to write them out separately, like `--reverse --unique`.

## Option parameters

Some options need you to supply an extra piece of information called a parameter directly after them to work.

In `ncal`, the `-A` option prints a set number of months _after_ the current one, and `-B` does the same for the months _before_. You can write these with a space (like `-B 2`) or without a space (like `-B2`). Both work.

You can mix these parameters with regular flags, but if you do, keep the parameter-heavy options separate so the shell doesn't get confused. As a general rule, always put your options first, followed by your main arguments at the end.
