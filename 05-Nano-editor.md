# Introduction to Nano

Unlike massive graphical editors like VS Code, terminal editors let you work directly where your code runs. Nano is simple, fast, and does not require any manual customization.

To open or create a file, just type `nano` followed by the filename:

```bash
nano config.txt
```

If the file does not exist yet, Nano opens a blank workspace. It won't actually create the file on your disk until you save your progress. To save, you have two options. You can use `Ctrl + O` that lets you change or confirm the filename before saving Or, you can just hit `Ctrl + S` to save directly to the current file without any prompt. Once you are done, `Ctrl + X` gets you back to your terminal prompt.

## Shortcuts

You can view the full shortcut menu by hitting `Ctrl + G`. One thing to watch out for is that Nano's shortcuts do not align with standard desktop apps. like, `Ctrl + V` pages down through your document instead of pasting text.

You will also see several shortcuts in the help menu that mention the Meta key, represented by the letter `M`. Since modern keyboards do not have a physical Meta key, you have to use a workaround depending on your operating system, windows and linux use the windows key and mac os uses the command key.

## Searching

To find a specific word, press `Ctrl + W`. Nano searches forward from where your cursor is sitting. If you want to search backward instead, hit Meta + `B`. You can also toggle case sensitivity by pressing Meta + `C`.

If you need to find and replace text, use `Ctrl + \`. Nano will ask you what to search for and what to replace it with. From there, you can approve changes one by one with `Y` or `N`, or swap them all at once by pressing `A`.

## Spell Checker

Nano has a built-in spell checker that you can trigger with `Ctrl + T`. However, it is often disabled by default. If you get an error when you try to use it, you will need to edit Nano's global configuration file.

---
