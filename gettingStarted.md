# Getting started with moFed:

## Create a project folder in your home directory (mine is called proj)
This is to put all your projects in. It may be advantageous to also create a component folder for component development work.

## xCode:
* https://itunes.apple.com/us/app/xcode/id497799835?mt=12
* Command line tools: put this in a terminal window `xcode-select --install`

## Install using NVM (preferred):
* NVM (preferred): https://github.com/creationix/nvm/blob/master/README.markdown
* Note: if using NVM don't install node, NVM will take care of that.
* Run `nvm install node` in a terminal

## Install Node using node download (if not using NVM):
* https://nodejs.org/en/
* Install N: https://github.com/tj/n

## Install Git:
* https://git-scm.com
* Your machine should have it already, but this will get the latest one.

## Git client:
* Command line: yep.
* Source Tree: https://www.sourcetreeapp.com (Atlassian’s client, integrates nicely with Bitbucket, our internal Git app)

## Atom:
* https://atom.io
* Don't forget to hit the `install shell commands` in the 'Atom' menu after it has started. This allows you to type `atom`, `atom .`, `atom someFile.js` and open then in atom from the terminal.

### plugins for atom:
* Linter: https://atom.io/packages/linter
* ESlint: https://atom.io/packages/linter-eslint
* ~ todo-show: https://atom.io/packages/todo-show ~ language-todo is now a default package.
* Terminal-plus: https://atom.io/packages/terminal-plus
* Tab-title: https://atom.io/packages/tab-title
* React: https://atom.io/packages/react
* Pigments: https://atom.io/packages/pigments
* Open-recent: https://atom.io/packages/open-recent
* Node-debugger: https://atom.io/packages/node-debugger
* Local-history: https://atom.io/packages/local-history
* Language-markdown: https://atom.io/packages/language-markdown
* File-icons: https://atom.io/packages/file-icons
* Emmet: https://atom.io/packages/emmet
* Custom-title: https://atom.io/packages/custom-title
* Atom-beautify: https://atom.io/packages/atom-beautify
* Column-selection: https://atom.io/packages/Sublime-Style-Column-Selection
* Filesize: https://atom.io/packages/filesize
* Mini-map: https://atom.io/packages/minimap
* Simple-drag-drop-text: https://atom.io/packages/simple-drag-drop-text

## Slack:
* CSP: http://ldscsp.slack.com
* LDS church: http://ldsics.slack.com
* UtahJS: http://utahjavascript.slack.com

## Misc apps:
* Sip: https://itunes.apple.com/us/app/sip/id507257563?mt=12
* xScope: http://xscopeapp.com
* Little Ipsum: http://dustinsenos.com/littleIpsum
* ~ Caffeine: https://itunes.apple.com/fm/app/caffeine/id411246225?mt=12 ~
* Amphetamine: https://itunes.apple.com/us/app/amphetamine/id937984704?mt=12&ign-mpt=uo%3D4
	* I have found this better than Xaffeine, but needs a very little bit of config

## Install LDSJS
The ldsjs library allows you to install starter kits for Javascript-based projects, like React.js or Angular.js. It also makes it simple to create new components within those projects. Ldsjs is maintained by the front-end stack team. 

1. Make sure you set NPM to use our local NPM repo first: `npm config set registry https://registry.npmjs.org/`
2. Install ldsjs globally: `npm i -g ldsjs`

## Get added to the moFed groups:
* Slack - #mofed channel in CSP
* LDS account group - Tell Colt you need to be added.
* Medium - https://medium.com/mofed
* Github - https://github.com/teamMoFed
* Gmail - TeamMoFed@gmail.com
* Twitter - @teamMoFed

## VPN info
* https://teams.ldschurch.org/wiki/wiki/pages/Connect%20to%20VPN%20Without%20AnyConnect.aspx

## Misc Stuff:

### Set screenshot folder
* Create folder on the desktop called `screenshots`.
* Terminal command: `defaults write com.apple.screencapture location ~/Desktop/screenshots`.
* Terminal command: `killall SystemUIServer`.
* Take a screenshot to test: `command + shift + 4` (`+ space` will take a screen shot of a selected app).
