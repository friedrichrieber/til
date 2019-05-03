# Vim Instant Markdown 

Did you ever made a Mistake in a ```README.md``` of Github Project because you did not check it before pushing it ? Do you think that Compiling it manually takes way to long ? 

Vim Instant Markdown is the right thing for you!

I compiles Markdown Code live in a Browser Windows from Vim

## How to install

(From the Github Page)

Installation
------------
You first need to have node.js with npm installed. Then:

- `[sudo] npm -g install instant-markdown-d`
- If you're on Linux, ensure the following packages are installed:
  - `xdg-utils`
  - `curl`
  - `nodejs-legacy` (for Debian-based systems)
- If you're on Windows, you will need into install [cURL][curl] and put it on your `%PATH%`.
- Copy the `after/ftplugin/markdown/instant-markdown.vim` file from this repo into your `~/.vim/after/ftplugin/markdown/` (creating directories as necessary), or follow your vim package manager's instructions.
- Ensure you have the line `filetype plugin on` in your `.vimrc`
- Open a markdown file in vim and enjoy!


Npm is a package Manger for Javascript. And i installed it from my default vim Plugin Manager.

## Pictures

![Use Case](/til/raw/master/media/vim_instant_markdown.png)


## Source 

- https://github.com/suan/vim-instant-markdown
