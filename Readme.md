# Learn Node Starter Kit
Written by William Kasel

## Prerequisites
- Install Node JS (see checklist below for mac version), [pc node version](https://www.guru99.com/download-install-node-js.html)
- Some kind of text editor/IDE, I use [Atom](https://atom.io) it's technically an extensible text-editor, alternatives are [sublime](asd), [vscode](https://code.visualstudio.com/), and [Webstorm by JetBrains](https://www.jetbrains.com/webstorm/) Webstorm is very good, and a true IDE like vs code, but it's not free.

## Cheatsheet
- `cd` change directory in terminal
- `rm` delete files in terminal
- `rm -rf` deletes directories (careful, NO RECYCLE BIN, GONEEEEE)
- `vim somefile.js` open in edit mode

## Checklist
1. Do you Have `brew` installed? To test open terminal and type `which brew`.
  - yes, continue to 3.
2. Install Brew:
  - [full directions here](https://changelog.com/posts/install-node-js-with-homebrew-on-os-x)
  - Copy & paste this into terminal `/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`
  - type `brew update`.
  - (Optionally) run `brew doctor`, if you like, it's good practice as it clean up any symbolic links (sym links). Next
  - type `vim ~/.bash_profile` (if you get any errors, ensure the bash_profile exists, if not type `touch ~/.bash_profile`)
  - to edit in vim, you have to hit the letter `i`, it's kind of weird as you have to key around to make edits. `i` pulls up interactive mode and allows you to make edits.
  - paste `export PATH="/usr/local/bin:$PATH"` into your bash_profile. Hit `esc` (escape key to exit interactive mode), then `:wq` (write + quit). If you screw something up and want to restart, just hit `esc` then `:q` (no write, just quit)
  - in terminal type `brew install node`
  - you now have node installed.
  - quick note, I recommend working in some directory inside your `~/` directory.
  - in terminal, run `node -v`, this is your node version. Also, ensure NPM installed correctly via `npm -v`.
  - a few notes sometimes you might get issues depending what features of Node.js packages are using, so it's also recommended you install xcode dev tools via `xcode-select --install`, then `sudo xcode-select --switch /Library/Developer/CommandLineTools` [full article](https://github.com/nodejs/node-gyp/issues/569)
3. Git Clone this repo, `cd` to the directory name via `cd learn-node-starter-kit` type `npm install` (note: `npm` is your node package manager, it's your go-to tool to install anything, everything, run tasks, and various scripts)

> _Checkpoint_: you now have Node setup, and a repository cloned

## Learning Your way around
  - Most node apps are setup with an entry file, sometimes named index.js, or other times called app.js, other times it's called server.js. It kind of depends on the layout.
  - `package.json` is how we maintain your dependencies, describe a package, and how we define scripts to run via the `npm run (name of command)` command.


## Getting Started
 - Ok, so you've cloned this repo, you've got node installed, let's write some code. 
