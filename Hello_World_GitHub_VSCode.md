# Hello World: Getting Started with GitHub and VS Code

In this project you will set up Git, GitHub, and Visual Studio Code, then build and publish your first repository: a small "Hello, World!" program.

**You can do everything in this tutorial with a free GitHub account.** You do not need to pay for anything. If you are a student, you can also apply for the GitHub Student Developer Pack. It unlocks GitHub Pro, Copilot Student, and dozens of partner tools at no cost. See [GitHub_Student_Developer_Pack.md](GitHub_Student_Developer_Pack.md) for how to set it up.

## What you will learn

By the end of this project, you will be able to:

- **Set up your tools.** Install Git and VS Code, and connect VS Code to your GitHub account.
- **Create a repository.** Turn a folder on your computer into a Git repository.
- **Commit changes.** Save snapshots of your work with clear messages.
- **Publish to GitHub.** Push your project to GitHub so it is backed up and shareable.
- **Update your project.** Make a change, commit it, and sync it to GitHub.

## What you need

- A computer running Windows, macOS, or Linux
- An email address (your school email works, and you will need it later for student benefits)
- About 45 minutes

## Key terms

| Term | Meaning |
| --- | --- |
| **Git** | A tool on your computer that tracks changes to files over time |
| **GitHub** | A website that stores Git projects online so you can back them up, share them, and work with others |
| **Repository (repo)** | A project folder that Git tracks, including its full history |
| **Commit** | A saved snapshot of your files, with a message describing what changed |
| **Push** | Sending your commits from your computer to GitHub |
| **Pull** | Bringing commits from GitHub down to your computer |

---

## Part 1: Create your GitHub account

1. Go to [github.com/signup](https://github.com/signup).
2. Enter your email, a password, and a username. Pick a professional username, because it appears in every link to your work.
3. Verify your email address when GitHub asks you to.
4. When asked to choose a plan, choose **Free**.
5. **Turn on two-factor authentication (2FA).** Go to **Settings > Password and authentication** and set it up with an authenticator app. GitHub requires 2FA for most accounts that contribute code, and you will need it for student benefits.

> **Tip:** If you are a student, add your school email under **Settings > Emails** now and verify it. That makes the student application in the other tutorial faster.

## Part 2: Install Git

**Windows**

1. Download Git from [git-scm.com/downloads](https://git-scm.com/downloads).
2. Run the installer. The default options are fine.

**macOS**

1. Open **Terminal** and run `git --version`.
2. If Git is not installed, macOS will offer to install the Command Line Developer Tools. Accept.

**Linux (Debian or Ubuntu)**

```bash
sudo apt update && sudo apt install git
```

**Check that it worked.** Open a terminal and run:

```bash
git --version
```

You should see a version number, such as `git version 2.x.x`.

**Tell Git who you are.** These details are attached to every commit you make. Use the same email as your GitHub account.

```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

## Part 3: Install VS Code and sign in to GitHub

1. Download and install VS Code from [code.visualstudio.com](https://code.visualstudio.com/).
2. Open VS Code.
3. Click the **Accounts** icon (the person icon) in the lower-left corner.
4. Choose **Sign in with GitHub to use GitHub Copilot** or **Sign in to Sync Settings**. Either option signs you in to GitHub.
5. Your browser opens. Approve the request, then return to VS Code.

> **Optional:** To run the Python version of Hello World, install Python from [python.org](https://www.python.org/downloads/) and the **Python** extension in VS Code (**Extensions** view, `Ctrl+Shift+X` or `Cmd+Shift+X`).

## Part 4: Build Hello World

1. Create a new folder on your computer named `hello-world`.
2. In VS Code, choose **File > Open Folder** and open `hello-world`.
3. Create a file named `hello.py` with this line:

   ```python
   print("Hello, World!")
   ```

4. Create a file named `README.md` with this content:

   ```markdown
   # Hello World

   My first GitHub repository, built with VS Code.
   ```

5. Run the program. Open the terminal with **Terminal > New Terminal**, then run:

   ```bash
   python hello.py
   ```

   On macOS or Linux, you may need `python3 hello.py`. You should see `Hello, World!`.

> **No Python?** You can do the rest of this tutorial with only the README. Git and GitHub work with any kind of file.

## Part 5: Make your first commit

1. Click the **Source Control** icon in the left sidebar (`Ctrl+Shift+G` or `Cmd+Shift+G`).
2. Click **Initialize Repository**. Git now tracks this folder.
3. Your two files appear under **Changes**. Hover over **Changes** and click **+** to stage them. Staging means "include these files in the next commit."
4. Type a commit message in the box at the top, such as `Add hello world program and README`.
5. Click **Commit**.

You have saved your first snapshot. So far it exists only on your computer.

## Part 6: Publish to GitHub

1. In the Source Control view, click **Publish Branch**.
2. Choose **Publish to GitHub public repository** so others can see it, or **private repository** to keep it to yourself. Both are free.
3. Wait for VS Code to finish. A notification offers **Open on GitHub**. Click it.

You should see your repository on GitHub with `hello.py` and `README.md`. GitHub displays the README on the repository's main page.

## Part 7: Make a change and sync it

1. In VS Code, edit `hello.py`:

   ```python
   name = "GitHub"
   print(f"Hello, {name}!")
   ```

2. Save the file. In Source Control, the file shows an **M** for "modified."
3. Stage it, write the message `Greet by name`, and click **Commit**.
4. Click **Sync Changes** to push the commit to GitHub.
5. Refresh your repository on GitHub. Click the commit count (for example, **2 Commits**) to see both snapshots in your history.

## Part 8 (optional): Try GitHub Copilot

GitHub Copilot is an AI coding assistant built into VS Code. The free Copilot plan works with any GitHub account and includes up to 2,000 code completions a month, plus limited chat. Verified students get **Copilot Student** instead, with unlimited completions.

1. Sign in to GitHub in VS Code (Part 3).
2. Follow the prompt to enable Copilot, if VS Code shows one.
3. In `hello.py`, type a comment such as `# print the numbers 1 to 5` and press Enter. Copilot suggests code in gray text. Press **Tab** to accept it.

---

## Checklist

When you finish, you should have:

- [ ] A GitHub account with 2FA turned on
- [ ] Git installed and set up with your name and email
- [ ] VS Code signed in to GitHub
- [ ] A `hello-world` repository on GitHub with at least two commits
- [ ] The repository link, to share or submit

## Free account vs. student account

Everything in this tutorial works on a free account. The Student Developer Pack adds more.

| Feature | Free account | With the Student Developer Pack |
| --- | --- | --- |
| Public and private repositories | Unlimited | Unlimited |
| GitHub plan | Free | GitHub Pro, free while you're a student |
| Codespaces (cloud dev environments) | 120 core hours and 15 GB storage per month | 180 core hours and 20 GB storage per month |
| GitHub Actions (automation) | 2,000 minutes per month | 3,000 minutes per month |
| GitHub Copilot | Copilot Free: up to 2,000 completions per month, limited chat | Copilot Student: unlimited completions, limited chat and agent use |
| Pages, wikis, protected branches in private repos | Public repos only | Included |
| Partner tools (JetBrains IDEs, free domains, cloud credits, learning platforms) | Not included | Included |

**Next step:** Follow [GitHub_Student_Developer_Pack.md](GitHub_Student_Developer_Pack.md) to unlock the student benefits.

## Troubleshooting

| Problem | Fix |
| --- | --- |
| `git` is not recognized | Restart VS Code, or your computer, after installing Git so the terminal picks it up. |
| VS Code asks for your name and email when you commit | Run the two `git config --global` commands in Part 2. |
| `python` is not recognized | Try `python3`, or reinstall Python and check **Add Python to PATH** (Windows). |
| Publish fails with a permissions error | Sign out of GitHub in VS Code (**Accounts** icon) and sign back in. |

## Sources

Details checked October 2026. GitHub's plans and limits change, so confirm current numbers at these links.

- [About GitHub's plans](https://docs.github.com/en/get-started/learning-about-github/githubs-plans)
- [Plans for GitHub Copilot](https://docs.github.com/en/copilot/concepts/billing/individual-plans)
- [GitHub Student Developer Pack](https://education.github.com/pack)
