Laptop
======

Laptop is a script to set up a macOS laptop for web and mobile development.

It can be run multiple times on the same machine safely.
It installs, upgrades, or skips packages
based on what is already installed on the machine.

Requirements
------------

Supported Operation System:

  * MacOS Monterey (12.01) - Apple M1 Processor

  Older versions may work but aren't regularly tested.
  Bug reports for older versions are welcome.

Install
-------

Download the script:

```sh
curl --remote-name https://raw.githubusercontent.com/wildcats-io/laptop/main/mac
```

Review the script (avoid running scripts you haven't read!):

```sh
less mac
```

Execute the downloaded script:

```sh
sh mac 2>&1 | tee ~/laptop.log
```

Optionally, review the log:

```sh
less ~/laptop.log
```

Debugging
---------

Your last Laptop run will be saved to `~/laptop.log`.
Read through it to see if you can debug the issue yourself.

If not, copy the lines where the script failed into a [new GitHub Issue](https://github.com/wildcats-io/laptop/issues/new).
Or, cut & paste the entire output into the issue.

If you see this error:

```sh
zsh compinit: insecure directories, run compaudit for list.
Ignore insecure directories and continue [y] or abort compinit [n]? 
```

You can fix it with the following command:

```sh
compaudit | xargs chmod g-w
```


What it sets up
---------------

Packages:

* [autojump] - command-line tools to jump to frequently used directories
* [bat] - clone of `cat(1)` with syntax highlighting and Git integration
* [exa] - modern replacement for `ls`
* [fd] - a simple, fast, and user-friendly alternative to `find`
* [fzf] - command-line fuzzy-finder
* [gh] - to work with GitHub on the CLI
* [git] - version control
* [git-delta] - syntax-highlighting for git & diff output
* [git-flow-avh] - to help you use Git-Flow based on [Vincent Driessen's branching model]
* [glab] - to work with GitLab on the CLI
* [glow] - render markdown on the CLI
* [jq] - a lightweight & flexible command-line JSON processor
* [n] - to manage versions of node JS
* [neofetch] - a fast, highly customizable system info script
* [neovim] - ambitious Vim-fork focused on extensibility and agility
* [python3] - Python 3.x
* [rcm] - rc file (dotfile) management
* [sngrep] - tool for displaying SIP calls message flows from CLI
* [starship] - cross-shell prompt
* [tmux] - terminal multiplexer
* [zsh-autosuggestions] - fish-like fast/unobtrusive autosuggestions for zsh
* [zsh-completions] - additional completion definitions for zsh
* [zsh-history-substring-search] - fish-like history search
* [zsh-syntax-highlighting] - fish-like syntax highlighting for zsh
* [font-hack-nerd-font], [font-meslo-lg-nerd-font], [font-sauce-code-pro-nerd-font] - nerd fonts, developer-targeted fonts patched with a glyphs & icons

Applications:

* [alacritty] - a GPU-accelerated terminal emulator
* [android-file-transfer] - transfer files from and to an Android smartphone
* [android-studio] - tools for building Android applications
* [appcleaner] - free application uninstaller
* [blockblock] - app to monitor common persistence locations
* [brave-browser] - web browser focusing on privacy
* [discord] - voice and text chat software
* [docker] - pack, ship and run any application as a lightweight container
* [google-drive] - client for the Google Drive storage service
* [hiddenbar] - utility to hide menu bar items
* [iina] - open-source media player
* [insomnia] - rest & graphql client (alternative to postman)
* [key-codes] - display key code, unicode value and modifier keys state for any key combination
* [lulu] - open-source firewall to block unknown outgoing connections
* [rectangle] - window tiling tools for macOS
* [slack] - team communication and collaboration software
* [sourcetree] - graphical client for Git version control
* [spotify] - music streaming service
* [stats] - macOS system monitor in your menu bar
* [suspicious-package] - app to inspect macOS Installer Packages
* [teamviewer] - remote access and connectivity software
* [telegram] - messaging app
* [visual-studio-code] - open-source code editor
* [zoom] - video communication and virtual meeting platform

It should take less than 15 minutes to install from scratch (depends on your machine), and about 2 seconds for subsequent runs.


[Vincent Driessen's branching model]: https://nvie.com/posts/a-successful-git-branching-model/

[autojump]: https://github.com/wting/autojump
[bat]: https://github.com/sharkdp/bat
[exa]: https://the.exa.website/
[fd]: https://github.com/sharkdp/fd
[fzf]: https://github.com/junegunn/fzf
[gh]: https://github.com/cli/cli
[git]: https://git-scm.com
[git-delta]: https://github.com/dandavison/delta
[git-flow-avh]: https://github.com/petervanderdoes/gitflow-avh
[glab]: https://github.com/profclems/glab
[glow]: https://github.com/charmbracelet/glow
[jq]: https://stedolan.github.io/jq/
[n]: https://www.npmjs.com/package/n
[neofetch]: https://github.com/dylanaraps/neofetch
[neovim]: https://neovim.io/
[python3]: https://www.python.org/
[rcm]: https://github.com/thoughtbot/rcm/
[sngrep]: https://github.com/irontec/sngrep
[starship]: https://starship.rs/
[tmux]: https://tmux.github.io/
[zsh-autosuggestions]: https://github.com/zsh-users/zsh-autosuggestions
[zsh-completions]: https://github.com/zsh-users/zsh-completions
[zsh-history-substring-search]: https://github.com/zsh-users/zsh-history-substring-search
[zsh-syntax-highlighting]: https://github.com/zsh-users/zsh-syntax-highlighting
[font-hack-nerd-font]: https://www.nerdfonts.com/
[font-meslo-lg-nerd-font]: https://www.nerdfonts.com/
[font-sauce-code-pro-nerd-font]: https://www.nerdfonts.com/

[alacritty]: https://github.com/alacritty/alacritty/
[android-file-transfer]: https://www.android.com/filetransfer/
[android-studio]: https://developer.android.com/studio/
[appcleaner]: https://freemacsoft.net/appcleaner/
[blockblock]: https://objective-see.com/products/blockblock.html
[brave-browser]: https://brave.com/
[discord]: https://discord.com/
[docker]: https://www.docker.com/
[google-drive]: https://www.google.com/drive/
[hiddenbar]: https://github.com/dwarvesf/hidden/
[iina]: https://iina.io/
[insomnia]: https://insomnia.rest/
[key-codes]: https://manytricks.com/keycodes/
[lulu]: https://objective-see.com/products/lulu.html
[rectangle]: https://github.com/rxhanson/Rectangle
[slack]: https://slack.com/
[sourcetree]: https://www.sourcetreeapp.com/
[spotify]: https://www.spotify.com/
[stats]: https://github.com/exelban/stats
[suspicious-package]: https://www.mothersruin.com/software/SuspiciousPackage/
[teamviewer]: https://www.teamviewer.com/
[telegram]: https://macos.telegram.org/
[visual-studio-code]: https://code.visualstudio.com/
[zoom]: https://www.zoom.us/

Contributing
------------

Edit the `mac` file.
Document in the `README.md` file.
Follow shell style guidelines by using [ShellCheck] and [Syntastic].

```sh
brew install shellcheck
```

[ShellCheck]: http://www.shellcheck.net/about.html
[Syntastic]: https://github.com/scrooloose/syntastic

### Credits

This laptop script is based on and inspired by [thoughtbot's laptop].

[thoughtbot's laptop]: https://github.com/thoughtbot/laptop

License
-------

Original Laptop script © 2011-2020 thoughtbot, inc.
