# Setting Up VS Code: A Beginner's Guide

Visual Studio Code (usually just called "VS Code") is a free code editor used by millions of professional developers — and it's also a great place to start as a complete beginner. This tutorial walks you through installing it, getting comfortable with the interface, and setting up a small set of extensions that make writing code noticeably easier when you're just starting out.

> **Goal:** Install VS Code, learn your way around it, and set up a handful of beginner-friendly extensions — so your editor is ready before you write your first real program.

This covers Windows, macOS, and Linux. Follow the steps for whichever system you're using.

---

## Before You Start

- A computer with an internet connection and about 15 minutes.
- Permission to install software on that computer (on a school or work computer, you may need an administrator password — ask first if you're not sure).
- Nothing else. You do not need to know how to code yet, and VS Code itself is completely free.

---

## Step 1 — Install VS Code

### Windows

1. Go to [code.visualstudio.com](https://code.visualstudio.com) and click the download button (it should detect Windows automatically).
2. Open the downloaded installer and run through the setup wizard.
3. On the "Select Additional Tasks" screen, check **"Add to PATH"** — this lets you open VS Code by typing `code` in a terminal later, which several extensions and tutorials assume you can do. Checking "Add 'Open with Code' action" is also handy — it adds VS Code to your right-click menu in File Explorer.
4. Finish the install and launch VS Code.

### macOS

1. Go to [code.visualstudio.com](https://code.visualstudio.com) and download the Mac version.
2. Open the downloaded `.zip` file, then drag the **Visual Studio Code** app into your **Applications** folder.
3. Open it from Applications. The first time, macOS may warn you it's an app downloaded from the internet — click **Open** to confirm.
4. Optional but recommended: open VS Code, press `Cmd+Shift+P` to open the Command Palette, type **"Shell Command"**, and select **"Shell Command: Install 'code' command in PATH."** This lets you type `code` in Terminal to open VS Code later.

### Linux

Pick whichever matches your system:

- **Debian/Ubuntu:** download the `.deb` package from [code.visualstudio.com](https://code.visualstudio.com) and install it, or run:
  ```
  sudo apt update
  sudo apt install code
  ```
  (if the `code` package isn't found, you may need to add Microsoft's repository first — the download page has instructions).
- **Fedora/RHEL:** download the `.rpm` package, or run `sudo dnf install code`.
- **Any distro:** VS Code is also available as a Snap (`sudo snap install code --classic`) or Flatpak.

---

## Step 2 — Take a Tour of the Interface

Open VS Code and take a minute to locate these pieces before doing anything else:

- **Activity Bar** — the strip of icons on the far left: Explorer (your files), Search, Source Control, Run and Debug, and Extensions. This is how you switch between the editor's major tools.
- **Side Bar** — opens next to the Activity Bar and shows whatever you selected (usually your project's file list).
- **Editor** — the big area in the middle where your actual code appears. You can open multiple files as tabs across the top.
- **Panel** — along the bottom; this is where the integrated **Terminal** lives, along with error/warning output. Open or close it with `` Ctrl+` `` (Windows/Linux) or `` Cmd+` `` (Mac).
- **Status Bar** — the thin strip along the very bottom, showing things like which programming language the current file is using.
- **Command Palette** — press `Ctrl+Shift+P` (Windows/Linux) or `Cmd+Shift+P` (Mac) any time you're not sure how to do something. Type what you're trying to do in plain English and VS Code will usually find the command for you. This is the single most useful shortcut to remember.

Try this now: go to **File → Open Folder**, create (or pick) an empty folder on your computer, and open it. That folder is now your "project" — you'll see it appear in the Explorer on the left. Most of your work in VS Code starts with opening a folder this way.

---

## Step 3 — A Few Beginner-Friendly Settings

These aren't required, but they remove some early friction:

- **Auto Save** — go to **File → Auto Save** and turn it on. As a beginner, this saves you from the classic "why isn't my code doing anything" moment that's actually just a forgotten `Ctrl+S`.
- **Color theme** — press `Ctrl+K` then `Ctrl+T` (or `Cmd+K` then `Cmd+T` on Mac) to preview and pick a theme. Pick whatever's easiest on your eyes; it has zero effect on how your code runs.
- **Font size** — open Settings with `Ctrl+,` (or `Cmd+,`) and search for "font size" if the default text is too small or large.

---

## Step 4 — Install Extensions

Extensions add features VS Code doesn't have out of the box — everything from language support to spell-checking. To install one:

1. Click the **Extensions** icon in the Activity Bar (or press `Ctrl+Shift+X` / `Cmd+Shift+X`).
2. Type the extension's name into the search box.
3. Click **Install** on the correct result (check the publisher name against the tables below — popular extensions sometimes have unofficial lookalikes).

### Essentials (install these regardless of what you're learning)

| Extension | Publisher | Why it helps a beginner |
|---|---|---|
| **Error Lens** | Alexander | Shows errors and warnings directly on the line that has them, instead of only in a separate panel you might not notice. |
| **Prettier – Code formatter** | Prettier | Automatically tidies up your code's spacing and indentation so it's readable — one less thing to think about while you're learning syntax. |
| **Code Spell Checker** | Street Side Software | Catches typos in your code and comments (misspelled variable names are a very common beginner bug). |
| **Indent Rainbow** | oderwat | Colors matching indentation levels, which makes nested code (loops inside functions, etc.) much easier to read at a glance. |
| **Material Icon Theme** | Philipp Kief | Gives each file type a distinct, recognizable icon in the file list — small, but it genuinely speeds up navigating a project. |

### If you're learning Python

| Extension | Publisher | Why it helps |
|---|---|---|
| **Python** | Microsoft | The core extension for writing and running Python — adds syntax highlighting, autocomplete, and a Run button. Installing it also installs **Pylance**, which powers the autocomplete and inline type checking. |
| **Jupyter** | Microsoft | Lets you open and run `.ipynb` notebook files directly in VS Code, with the same interactive, cell-by-cell experience as Jupyter itself. |

### If you're learning web development (HTML/CSS/JavaScript)

| Extension | Publisher | Why it helps |
|---|---|---|
| **Live Server** | Ritwick Dey | Adds a "Go Live" button that opens your HTML file in a browser and automatically refreshes it every time you save — no more manually reloading the page. |
| **HTML CSS Support** | ecmel | Autocompletes CSS class and ID names inside your HTML as you type. |
| **Auto Rename Tag** | Jun Han | When you rename an opening HTML tag (like `<div>`), automatically renames the matching closing tag too. |

### Optional: AI-assisted coding

Once you're comfortable with the basics, some beginners also use an AI coding extension inside VS Code itself — for example the **Claude Code** or **GitHub Copilot** extensions, which can suggest code as you type or answer questions about your project. These are optional and not necessary to get started; if you've been working through the AI-prompting tutorials in this series, this is simply that same skill living inside your editor instead of a separate browser tab.

---

## Step 5 — Try It Yourself

Confirm everything actually works before moving on:

**If you installed the Python extension:**
1. In your open folder, create a new file named `hello.py`.
2. Type: `print("Hello, world!")`
3. Click the **Run** (▶) button in the top-right corner of the editor, or right-click in the file and choose **Run Python File in Terminal**.
4. You should see `Hello, world!` appear in the terminal at the bottom.

**If you installed Live Server:**
1. Create a new file named `index.html` with some basic content, for example `<h1>Hello, world!</h1>`.
2. Right-click anywhere in the file and choose **Open with Live Server** (or click **Go Live** in the status bar).
3. Your default browser should open showing your page. Edit the file, save it, and watch the browser update on its own.

If either of these worked, your setup is good to go — and if you've already been through the other tutorials in this series (the browser game or the data dashboard), you now have a proper editor to open those project files in instead of a plain text editor.

---

## Troubleshooting

- **"`python` is not recognized" / "`python3`: command not found" in the terminal.** On Windows, reinstall Python from [python.org](https://python.org) and make sure **"Add python.exe to PATH"** is checked during setup. On Mac/Linux, try `python3` instead of `python` — many systems use that name instead.
- **An extension's icon or button isn't showing up after installing it.** Reload the window: open the Command Palette (`Ctrl+Shift+P` / `Cmd+Shift+P`) and run **"Developer: Reload Window."**
- **Typing `code` in a terminal does nothing (Mac/Linux).** Revisit the PATH step in Step 1 — for Mac, it's the Command Palette's "Shell Command: Install 'code' command in PATH."
- **The Run button doesn't appear for a Python file.** Check the bottom-right of the Status Bar — VS Code needs a Python interpreter selected. Click there (or run **"Python: Select Interpreter"** from the Command Palette) and pick the version of Python installed on your system.

---

## What You're Really Learning

- Why developers use a dedicated code editor instead of a plain text editor like Notepad or TextEdit
- How extensions add capability to a tool without bloating what you don't need
- How to navigate a development environment on your own, using the Command Palette as a safety net
- The habit of verifying a new setup actually works with a trivial test, before building anything real on top of it
