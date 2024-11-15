# Setup for Developments

## Basic Stuffs

- Get work email
- Create Apple ID
- Update MacBook
- Set up Mac from Settings

## Application Install

- ARC
- Chrome
- Docker
- Microsoft package from App Store
- Microsoft Teams
- Postman
- Figma
- Postgres
- Draw.io
- SQL Server Management Studio (SSMS)
- Azure Data Studio
- Slack / Signal / Discord
- SourceTree / Gitkraken
- Webex

## VS Code Extensions

### Common 

- CodeSnap
- Learn with Sumit theme
- GitLens
- GitHub Copilot
- Git History
- Docker
- In Your Face
- Lorem Ipsum
- Markdown All in One
- Sublime Text Keymap and Settings Importer
- vscode-faker
- YAML

### Frontend

- Babel
- Es7+
- TypeScript, JavaScript
- Version Lens
- Eslint
- Prettier
- Live Server
- Npm intelligence
- Tailwind CSS intelligence
- Node module intelligence
- Auto import cost
- Auto rename tag
- Auto Close Tag
- Better comment
- Peacock
- Project manager
- Intellicode
- VSCode icons / material icons
- Path Intellisense

### Backend

- .Net Extension Pack
- .Net Install Tool
- C#
- C# Dev Kit
- C# Extensions
- C# Namespace Autocompletion
- CSharpier - Code formatter
- Error Lens
- IntelliCode for C# dev kit
- Ionide for F#
- SQL Server (mssql)

## Terminal / CLI Setup

- Install Xcode Command Line Tools

```bash
xcode-select --install
```
- Install iTerm2

```bash
brew install --cask iterm2
```

- Install Azure CLI
- Install Git
- Set up Git command aliases
- Install Homebrew
- Install Node.js
- Install NVM (Node Version Manager)
- Install Yarn globally

### Oh-my-zsh

- For setup guide, follw this - [Wiki](https://github.com/ohmyzsh/ohmyzsh/wiki/)

- Install PowerLevel10K Theme for Oh My Zsh [Powerlevel10k](https://gist.github.com/n1snt/454b879b8f0b7995740ae04c5fb5b7df)


```bash
git clone https://github.com/romkatv/powerlevel10k.git $ZSH_CUSTOM/themes/powerlevel10k
```
- Update .zshrc file

```bash
# Enable Powerlevel10k instant prompt. Should stay close to the top of ~/.zshrc.
# Initialization code that may require console input (password prompts, [y/n]
# confirmations, etc.) must go above this block; everything else may go below.
if [[ -r "${XDG_CACHE_HOME:-$HOME/.cache}/p10k-instant-prompt-${(%):-%n}.zsh" ]]; then
  source "${XDG_CACHE_HOME:-$HOME/.cache}/p10k-instant-prompt-${(%):-%n}.zsh"
fi

# If you come from bash you might have to change your $PATH.
# export PATH=$HOME/bin:/usr/local/bin:$PATH

# Path to your oh-my-zsh installation.
export ZSH="$HOME/.oh-my-zsh"

# Set name of the theme to load --- if set to "random", it will
# load a random theme each time oh-my-zsh is loaded, in which case,
# to know which specific one was loaded, run: echo $RANDOM_THEME
# See https://github.com/ohmyzsh/ohmyzsh/wiki/Themes
# ZSH_THEME="robbyrussell"
ZSH_THEME="powerlevel10k/powerlevel10k"

# Set list of themes to pick from when loading at random
# Setting this variable when ZSH_THEME=random will cause zsh to load
# a theme from this variable instead of looking in $ZSH/themes/
# If set to an empty array, this variable will have no effect.
# ZSH_THEME_RANDOM_CANDIDATES=( "robbyrussell" "agnoster" )

# Uncomment the following line to use case-sensitive completion.
# CASE_SENSITIVE="true"

# Uncomment the following line to use hyphen-insensitive completion.
# Case-sensitive completion must be off. _ and - will be interchangeable.
# HYPHEN_INSENSITIVE="true"

# Uncomment one of the following lines to change the auto-update behavior
# zstyle ':omz:update' mode disabled  # disable automatic updates
# zstyle ':omz:update' mode auto      # update automatically without asking
# zstyle ':omz:update' mode reminder  # just remind me to update when it's time

# Uncomment the following line to change how often to auto-update (in days).
# zstyle ':omz:update' frequency 13

# Uncomment the following line if pasting URLs and other text is messed up.
# DISABLE_MAGIC_FUNCTIONS="true"

# Uncomment the following line to disable colors in ls.
# DISABLE_LS_COLORS="true"

# Uncomment the following line to disable auto-setting terminal title.
# DISABLE_AUTO_TITLE="true"

# Uncomment the following line to enable command auto-correction.
# ENABLE_CORRECTION="true"

# Uncomment the following line to display red dots whilst waiting for completion.
# You can also set it to another string to have that shown instead of the default red dots.
# e.g. COMPLETION_WAITING_DOTS="%F{yellow}waiting...%f"
# Caution: this setting can cause issues with multiline prompts in zsh < 5.7.1 (see #5765)
# COMPLETION_WAITING_DOTS="true"

# Uncomment the following line if you want to disable marking untracked files
# under VCS as dirty. This makes repository status check for large repositories
# much, much faster.
# DISABLE_UNTRACKED_FILES_DIRTY="true"

# Uncomment the following line if you want to change the command execution time
# stamp shown in the history command output.
# You can set one of the optional three formats:
# "mm/dd/yyyy"|"dd.mm.yyyy"|"yyyy-mm-dd"
# or set a custom format using the strftime function format specifications,
# see 'man strftime' for details.
# HIST_STAMPS="mm/dd/yyyy"

# Would you like to use another custom folder than $ZSH/custom?
# ZSH_CUSTOM=/path/to/new-custom-folder

# Which plugins would you like to load?
# Standard plugins can be found in $ZSH/plugins/
# Custom plugins may be added to $ZSH_CUSTOM/plugins/
# Example format: plugins=(rails git textmate ruby lighthouse)
# Add wisely, as too many plugins slow down shell startup.
plugins=(git 
	zsh-autosuggestions 
	zsh-syntax-highlighting 
	fast-syntax-highlighting 
	zsh-autocomplete
	colorize
	docker
	docker-compose
	git
	macos
	node
	npm 
	nvm
	pip
	python
	pipenv
	postgres
	vscode
)

source $ZSH/oh-my-zsh.sh

# User configuration

# export MANPATH="/usr/local/man:$MANPATH"

# You may need to manually set your language environment
# export LANG=en_US.UTF-8

# Preferred editor for local and remote sessions
# if [[ -n $SSH_CONNECTION ]]; then
#   export EDITOR='vim'
# else
#   export EDITOR='mvim'
# fi

# Compilation flags
# export ARCHFLAGS="-arch x86_64"

# Set personal aliases, overriding those provided by oh-my-zsh libs,
# plugins, and themes. Aliases can be placed here, though oh-my-zsh
# users are encouraged to define aliases within the ZSH_CUSTOM folder.
# For a full list of active aliases, run `alias`.
#
# Example aliases
# alias zshconfig="mate ~/.zshrc"
# alias ohmyzsh="mate ~/.oh-my-zsh"

# To customize prompt, run `p10k configure` or edit ~/.p10k.zsh.
[[ ! -f ~/.p10k.zsh ]] || source ~/.p10k.zsh
```
- To reflect this change on your terminal, restart it or run this 
command `source ~/.zshrc`

## Update VSCode Terminal Settings

```json
{
  "editor.formatOnSave": true,
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": "explicit",
    "source.fixAll.tslint": "explicit",
    "source.organizeImports": "explicit"
  },
  "typescript.validate.enable": true,
  "javascript.validate.enable": true,
  "terminal.integrated.fontFamily": "FiraCode Nerd Font",
  "git.autofetch": true,
  "window.zoomLevel": 1,
  "workbench.colorTheme": "Learn with Sumit - Professional",
  "git.enableSmartCommit": true,
  "git.confirmSync": false,
  "explorer.confirmDragAndDrop": false,
  "editor.defaultFormatter": "GitHub.copilot",
  "javascript.updateImportsOnFileMove.enabled": "always",
  "explorer.confirmDelete": false,
  "[python]": {
    "editor.formatOnType": true
  },
  "[json]": {
    "editor.formatOnSave": true,
    "editor.defaultFormatter": "vscode.json-language-features"
  },
  "editor.largeFileOptimizations": true,
  "typescript.updateImportsOnFileMove.enabled": "always",
  "workbench.iconTheme": "vscode-icons",
  "terminal.integrated.defaultProfile.windows": "Git Bash",
  "azureResourceGroups.groupBy": "resourceGroup",
  "workbench.startupEditor": "none",
  "github.copilot.editor.enableAutoCompletions": true,
  "security.workspace.trust.untrustedFiles": "open",
  "editor.fontSize": 13,
  "git.ignoreRebaseWarning": true,
  "[csharp]": {
    "editor.defaultFormatter": "csharpier.csharpier-vscode"
  },
  "editor.fontFamily": "Consolas, 'Courier New', monospace, FiraCode Nerd Font",
  "azureResourceGroups.selectedSubscriptions": [],
  "files.exclude": {
    "**/bin": true,
    "**/obj": true
  },
  "window.newWindowProfile": "Default",
  "settingsSync.ignoredExtensions": [
    "sonarsource.sonarlint-vscode"
  ],
  "explorer.confirmPasteNative": false,
  "better-comments.multilineComments": true,
  "better-comments.highlightPlainText": false,
  "better-comments.tags": [
    {
      "tag": "!",
      "color": "#FF2D00",
      "strikethrough": false,
      "underline": false,
      "backgroundColor": "transparent",
      "bold": false,
      "italic": false
    },
    {
      "tag": "?",
      "color": "#3498DB",
      "strikethrough": false,
      "underline": false,
      "backgroundColor": "transparent",
      "bold": false,
      "italic": false
    },
    {
      "tag": "//",
      "color": "#474747",
      "strikethrough": true,
      "underline": false,
      "backgroundColor": "transparent",
      "bold": false,
      "italic": false
    },
    {
      "tag": "todo",
      "color": "#FF8C00",
      "strikethrough": false,
      "underline": false,
      "backgroundColor": "transparent",
      "bold": false,
      "italic": false
    },
    {
      "tag": "*",
      "color": "#98C379",
      "strikethrough": false,
      "underline": false,
      "backgroundColor": "transparent",
      "bold": false,
      "italic": false
    }
  ],
  "github.copilot.enable": {
    "*": true,
    "plaintext": false,
    "markdown": false,
    "scminput": false
  }
}
```
