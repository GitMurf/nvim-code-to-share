# Overview

I am going to keep this short and sweet... one thing I miss from writing directly in Obsidian as opposed to writing my notes in markdown files in Neovim terminal, is the ability to embed an iframe of the MDWA website to force myself to write for 3, 5, N minutes straight without stopping for too long.

See Most Dangerous Writing App website if you are not familiar with it here:

- Original GitHub project: https://github.com/maebert/themostdangerouswritingapp
- Current hosted provider: https://www.squibler.io/dangerous-writing-prompt-app

So I decided to hack together a way to do this in Neovim by creating a new window and empty buffer and replicate the behavior of MDWA! It is a simple 160 lines of code.

# Installation Instructions

I do NOT want to spend the time trying to make this into a full "real" plugin so all you need to do is simply paste the code from my `mdwa.lua` here on GitHub, into a lua file in your Neovim config (I just add it to my autocmds file) and make sure it loads on startup.

# Usage Instructions

To start a new MDWA session, just do the command `:MdwaNew` for the default 3 minute session or `:MdwaNew 7` as example for a 7 minute session (you can do any `n` integer for minutes).

# Demos

## Demo of MDWA 5 second inactivity causes buffer content to be lost

https://github.com/user-attachments/assets/a5b78140-0033-497d-85ce-fb047ca4f46d

## Demo of finishing 1 minute writing session successfully

TBD

# License

MIT... feel free to do whatever you want with the code! If someone wants to make this into a plugin, go for it!
