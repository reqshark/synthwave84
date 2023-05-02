# synthwave 1984
## mac os terminal theme

![synthwave_rad](rad_bg_preview.png)

## to install synthwave
  1. open mac os `terminal` settings
  2. go to profiles tab
  3. on the bottom left hit the `+` plus button to find `synthwave84.terminal` this repo directory
  4. to achieve a most radical terminal, set the background with the included `outrun_bg.jpg`

<sub>special note: to get it to look exactly like this you would need to first install my fork of [.bash-git-prompt](https://github.com/reqshark/bash-git-prompt) then with node installed for the user make sure to have `ip` installed global or in a random `node_modules` in your HOME dir so u can require it from user at shell login:</sub>
```bash
git clone https://github.com/reqshark/bash-git-prompt.git ~/.bash-git-prompt

# ------------------------------------------------------------------------
## steps for mac
echo -e "source $HOME/.bash-git-prompt/gitprompt.sh" >> "$HOME/.bash_profile"
npm i -g ip
# custom prompt w/ local ip addr display
echo -e 'export NODE_ENV=`node -e "process.stdout.write(require('ip').address())"`' >> "$HOME/.bash_profile"

# ------------------------------------------------------------------------
## steps for linux
echo -e "source $HOME/.bash-git-prompt/gitprompt.sh" >> "$HOME/.bashrc"
npm i -g ip
echo -e 'export NODE_ENV=`node -e "process.stdout.write(require('ip').address())"`' >> "$HOME/.bashrc"
```
# back  to the synthewave setup on mac os
this is where you export and add terminal profiles/themes on mac
![settings](settings.png)

# rad version
there are a couple different themes with a few minor differences (a few colors are flipped):
  1. `synthwave84.terminal`
  2. `synthwave84_rad_version.terminal`

![synthwave](screenshot.png)

print using [ccat](https://github.com/owenthereal/ccat) on the rad theme:

![rad](synthwave_rad.png)

a terminal selection of the ccat output:

![rad](synthwave_rad_selection.png)

edit with vim:

![vim](synthwave_vim.png)
