# Shell Basics

## Learning Objectives

- learning what the terminal and the shell are
- learning to navigate the file system using the shell and the terminal
- learning to create, rename, remove and move files and folders in the filesystem

---

## Shell and Terminal

You are probably used to using GUIs
([Graphical User Interfaces](https://en.wikipedia.org/wiki/Graphical_user_interface)) to interact
with computers.

Often times developers interact with computers using CLIs (Command Line Interfaces) which are text
based user interfaces. That means that you type commands to interact with the computer (create /
move / delete / edit files, install software, change system settings...).

This has the following reasons / advantages:

- Many tools don't have a GUI and can only be used as a CLI.
- You can write scripts (which consist of a number of commands) to automate processes and repetitive
  tasks and ensure they are being run exactly the same way every time they are executed.

On macOS we are using zsh (z shell) as the command interpreter.

By default it is run within the Terminal app. For this course we'll use iTerm and Visual Studio Code
as alternative terminal emulators.

- A shell (like zsh) is the command interpreter that runs and executes commands on your computer and
  outputs results.
- A terminal (like Terminal, iTerm, Visual Studio Code) is a text input and output environment
  (emulating a [hardware computer terminal](https://en.wikipedia.org/wiki/Computer_terminal)) that
  sends commands to the shell and displays its output.

### Basic Shell commands

| command            | functionality                                                              |
| ------------------ | -------------------------------------------------------------------------- |
| `ls`               | list the content of the current directory                                  |
| `cd <folder name>` | change directory into a folder                                             |
| `cd ..`            | change into the parent folder                                              |
| `cd ~`             | change into your home directory                                            |
| `pwd`              | print the current directory path                                           |
| `touch example.md` | create a file called "example.md"                                          |
| `mkdir newFolder`  | create a folder called "newFolder"                                         |
| `rm <file name>`   | delete a file permanently (there is no trash bin to recover files!)        |
| `open .`           | open the current folder in the finder                                      |
| `cat <file name>`  | prints the content of a specific file                                      |
| `curl <url>`       | prints the received content from the specified url. (try `curl ipinfo.io`) |

> 💡 There are a lot of commands for any sort of action you want to perform check out
> [this cheat cheet](https://github.com/RehanSaeed/Bash-Cheat-Sheet) to look up important commands.

---

## Resources

- [terminal basics](https://mrkaluzny.com/blog/terminal-101-getting-started-with-terminal/)
- [command line cheat sheet](https://github.com/0nn0/terminal-mac-cheatsheet#english-version)

---

# Challenges

## Terminal Setup

1. open the **spotlight search**: `cmd` `space`
2. open the terminal: `terminal`
3. install [homebrew](https://brew.sh/)
4. (accept installing Xcode Command Line Tools, takes some minutes to install)
5. install [powerlevel10k](https://github.com/romkatv/powerlevel10k#homebrew) via homebrew:
   ```bash
   brew install romkatv/powerlevel10k/powerlevel10k
   echo "source $(brew --prefix)/opt/powerlevel10k/powerlevel10k.zsh-theme" >>~/.zshrc
   ```
6. restart the terminal to enter the configuration or type
   ```bash
   p10k configure
   ```
7. configure the zsh theme as you like
8. change the font size of the terminal to 18px: `Terminal` -> `preferences` -> `Profiles` -> `Font`
   -> `Change...`

## VS Code installation

1. install VS Code and explain what in IDE is:
   ```bash
   brew install --cask visual-studio-code
   ```
1. install the prettier extension **Prettier - Code formatter** and explain what a code formatter
   does
1. Go to the VS Code settings and:
   - search for "default formatter" and set to prettier
   - search for "format on save" and hit checkbox
1. install the extension `Auto Rename Tag`
1. install the extension `Live Preview`

## Treasure Hunt

In this challenge you have to find the lost diamond of the ancient king of treasure island! Open the
**treasure-hunt.zip** that you received. Navigate through treasure island only with the terminal and
find the treasure! Use the following commands:

- use `cd` to change directories
- use `cd ..` to move out of the current folder
- use `ls` to look what is in the current folder
- use `cat` to see what is inside a markdown file
- use `pwd` to see your current directory path
