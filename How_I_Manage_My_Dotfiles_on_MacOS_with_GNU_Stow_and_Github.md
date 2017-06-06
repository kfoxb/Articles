# How I Manage My Dotfiles on MacOS with GNU Stow and Github

## One time setup

### create or fork a repo on github
- link to githubs dotfiles page
- link to creating a repo

## First time using stow

### installation
- using home brew
- other methods

### clone the repo to your home folder and add files
- if you have existing dotfiles create a folder and migrate them in to the dotfiles repo
```bash
#change to dotfiles directory
cd dotfiles
#make a folder named after the application inside the dotfiles directory
mkdir zsh
#move any config files or folders in your home directory into the directory you just created
mv ~/.zshrc zsh
```

- otherwise you can create a folder inside named after the application that you're creating dotfiles for

###Link the files with stow
```bash
stow zsh
```

### Other things to consider
- watch out for sensitive information
- make different branches for different operating systems
- unstow files
- store the folder elsewhere