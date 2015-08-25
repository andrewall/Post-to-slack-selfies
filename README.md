# Post-to-slack-selfies
Instructions and .bashrc snippet

## Setup

1. Download and install xcode (install via app store)
2. `imagesnap`  (brew installable) for taking web cam selfies
3. Generate your slack API token here: https://api.slack.com/web
4. Create a folder somewhere on your system and take note of it's location (mine is `~/Desktop/git\ commit\ images;`)
5. Copy over the snippet found in `.bashrc-snippet` file in this repo into your `~/.whateverYouHaverc` file (be it `~/.bachrc` (default) or `~/.zshrc`)
6. Put your slack API token from step 3. into `slackApiToken` variable in snippet (use double quotes e.g. `slackApiToken="1337";`)
7. Put your selfie directory from step 4. within `selfieDirectory` variable in snippet (no quotes e.g. `selfieDirectory=~/Desktop/git\ commit\ images;`)
8. Save then resource your shell using `source ~/.whateverYouHaverc` (e.g. `source ~/.zshrc`).  Alternatively open a new shell tab.
9. ????
10. Profit

## Usage

`git-commit "Your commit message here"`

Note: Don't you dare put `-m` when using this like I still do.  But if you mess this up simply rerun `git reset --soft HEAD~1`  (http://stackoverflow.com/questions/927358/how-do-you-undo-the-last-commit).

## Customize
File upload API: https://api.slack.com/methods/files.upload