# My favourite configuration, cheat code and so on [<img src="https://github.com/lonewolfnadhu/lonewolfnadhu/blob/main/Resources/Icons/auther-icon.png">](https://github.com/lonewolfnadhu/lonewolfnadhu/tree/main/Resources)
Created by [Nadir Shah](https://linktr.ee/lonewolfnadhu)


## #1  'Terminal' Configuration
```
[FYI: Configure 'Terminal' as below for better performance and making work faster]

Step #01: Make current user a root user
Type: dsenableroot

Step #02: Install ZSH via homebrew
Type: brew install zsh

Step #03: Make it your default shell
Type: chsh -s /bin/zsh

Step #04: Verify the shell
Type: echo $SHELL (Note: Check whether it prints '/usr/bin/zsh')

Step #05: Install 'Oh My Zsh'
Type: sudo sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"

Step #06: Clone 'PowerLeve10K theme'
Type: git clone https://github.com/romkatv/powerlevel10k.git $ZSH_CUSTOM/themes/powerlevel10k

Step #07: Clone 'autosuggestion'
Type: sudo git clone https://github.com/zsh-users/zsh-autosuggestions.git $ZSH_CUSTOM/plugins/zsh-autosuggestions

Step #08: Clone 'highlighting'
Type: sudo git clone https://github.com/zsh-users/zsh-syntax-highlighting.git $ZSH_CUSTOM/plugins/zsh-syntax-highlighting

Step #09: Open ".zshrc" and replace these sections / files
1. ZSH_THEME="powerlevel10k/powerlevel10k"
2. ENABLE_CORRECTION="true"
3. plugins=(git zsh-autosuggestions zsh-syntax-highlighting)

Step #10: To final configuration
Type: p10k configure

Reference: 
https://medium.com/@shivam1/make-your-terminal-beautiful-and-fast-with-zsh-shell-and-powerlevel10k-6484461c6efb
```


## #2  'VS Code' Configuration
```
[FYI: Install below 'VS Code' packages to make your IDE more stable and for better performance]

Package #01: 'React Native Tools'

Package #02: 'Babel JavaScript'

Package #03: 'ESLint'

Package #04: 'Prettier - Code formatter'

Package #05: 'Auto Close Tag'

Package #06: 'Auto Complete Tag'

Package #07: 'Auto Rename Tag'

Package #08: 'Color Highlight'

Package #09: 'Path Intellisense'

Package #10: 'Rainbow Brackets'

Package #11: 'SVG Viewer'

Package #12: 'TODO Highlight'

Package #13: 'change-case'

Package #14: 'Code Spell Checker'

Package #15: 'npm' and 'npm intellisense'

Package #16: 'Material Icon Theme' [Note: Theme for the 'Icons']

Package #17: 'Night Owl' [Note: Theme for the 'IDE']

Package #18: 'code .' [Note: To open 'VS Code']
```


### #3  Open an 'iOS Simulator'
```
Step #1: Type 'xcrun simctl list devices'
[FYI: List all 'iOS Simulators' / 'Physical Devices']

Step #2: Type 'open -a Simulator'
[FYI: To open ios simulator, Default will be 'iPhone 14']
```


### #4  Open an 'Android Emulator'
```
Step #1: Type 'adb devices'
FYI: List all 'Android Emulators' / 'Physical Devices']

Step #2: Type 'emulator -avd Pixel'
[FYI: To open android emulator named 'Pixel', if it doen't open type 'source ~/.bash_profile' then type 'emulator -avd Pixel' again]
```


### #5  'Git' Cheat Code
```
Tip #01: git --version   <<<OR>>>   git version
// Show git version

Tip #02: git help   <<<AND>>>   git help config
// Show general help and configuration help

Tip #03: PRESSS 'q'   <<<OR>>>   'Q'
// Exit to terminal

Tip #04: git config --global user.name "Nadir Shah"
// Configure git username as 'Nadir Shah' globally

Tip #05: git config --global user.email "lonewolfnadhu@gmail.com"
// Configure git email as 'lonewolfnadhu@gmail.com' globally

Tip #06: git config --global --list
// List out all global configuration settings

Tip #07: touch README.md
// Create a new file name 'README.md'

Tip #08: cat README.md
// Open 'README.md' file in terminal

Tip #09: vim README.md
// Open 'README.md' file in terminal
// PRESS 'i' to edit 'README.md' file
// PRESS 'esc' to go back to terminal file / exit from terminal
// ENTER ':wq' to save 'README.md' file

Tip #10: pwd
// Show current directory (folder) (present working directory (folder))

Tip #11: cd workspace
// Move to 'workspace' folder

Tip #12: ls
// Show files and folders in current directory (folder) without parameters, will list non-hidden folders and files

Tip #13: ls -a
// Show current files in that directory (folder) including hidden files

Tip #14: git init git-demo
// Create or initialise empty git repository

Tip #15: git status
// Modification or changes in current repository
// Show which files have been modified in the working directory (folder) and git's staging area

Tip #16: git add README.md
// Adds the new or newly modified 'README.md' file to git's staging area

Tip #17: git add .
// Adds all new or newly modified files to git's staging area

Tip #18: git commit -m "Initial Commit"
// Commits all files currently in git's staging area
// The '-m' parameter allows for a commit message directly from the command line

Tip #19: git commit -am "Adding some more items"
// Directly commit newly modified tracked files

Tip #20: clear
// Clear all commands from the terminal screen

Tip #21: git reset HEAD README.md
// "Unstage" the specified file from git's staging area

Tip #22: git checkout -- README.md
// Back out any changes made to the specified file and replace it with the version last committed in git

Tip #23: git log
// Git commit history

Tip #24:  git log --oneline --graph --decorate --color
// Much better compact view of git commit history

Tip #25: mkdir Demo
// Creating a new directory (folder) name 'Demo'

Tip #26: git rm Demo.md
// Deleting 'Demo.md' file

Tip #27: mv Demo.txt subfolder/
// Move 'Demo.txt' to 'subfolder/' directory (folder)

Tip #28: git remote -v
// List out all git repositories

Tip #29: which git
// Shows git location
```


### #6  Configuring 'SSH Authentication' with GitHub
```
Step #01: cd ~ 
// Go to the main user directory (folder)

Step #02: pwd
// Make sure we are in main directory

Step #03: cd .ssh
// Make sure there are no '.ssh' file

Step #04: mkdir .ssh
// Create '.ssh' file

Step #05: ssh-keygen -t rsa -C "lonewolfnadhu@gmail.com"
// Generate new ssh keygen
// Make sure we are in main directory

Step #06: ls -al
// Show all files in '.ssh' folder
// Make sure we have 'id_rsa' and 'id_rsa.pub' files in '.ssh' folder

Step #07: // Open 'id_rsa.pub' file, copy everthing and paste in github website where it shows to setup ssh key

Step #08: ssh -T git@github.com
// Connect to github over ssh protocol
```


## Connect with me [<img src="https://github.com/lonewolfnadhu/lonewolfnadhu/blob/main/Resources/Icons/projects-icon.png">](https://github.com/lonewolfnadhu/lonewolfnadhu/tree/main/Resources)
[<img src="https://github.com/lonewolfnadhu/lonewolfnadhu/blob/main/Resources/Icons/instagram-icon.png">](https://www.instagram.com/lonewolfnadhu/)
[<img src="https://github.com/lonewolfnadhu/lonewolfnadhu/blob/main/Resources/Icons/whatsapp-icon.png">](https://api.whatsapp.com/send?phone=07442013458&lang=en)
[<img src="https://github.com/lonewolfnadhu/lonewolfnadhu/blob/main/Resources/Icons/linkedin-icon.png">](https://www.linkedin.com/in/lonewolfnadhu/)
[<img src="https://github.com/lonewolfnadhu/lonewolfnadhu/blob/main/Resources/Icons/facebook-icon.png">](https://www.facebook.com/lonewolfnadhu/)
[<img src="https://github.com/lonewolfnadhu/lonewolfnadhu/blob/main/Resources/Icons/github-icon.png">](https://github.com/lonewolfnadhu)


Show your support!


Made with ❤️


Copyright © 2020-2023 [Nadir Shah](https://linktr.ee/lonewolfnadhu)
