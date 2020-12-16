# Bash Tools

> A compilation of various Bash scripts I've created on the fly to help me deal with life on a terminal.

***

## Installation:

Run the `install.sh` script as root **WHILE IN REPO DIRECTORY!** Root is really only required if you don't change the default path (/usr/local/bin). To set a home path, edit the `install.sh` script and change `temp_path` to whatever you want the symlink to run through. If you run as root user (not just sudo), make sure the repo itself is somewhere accessible by all accounts!

<br/>

## Updates:

There are 2 update options:

- Run the `update.sh` script provided with the repo.
> !!! MAKE SURE THE PATHS IN THE `update.sh` ARE CORRECT !!!

<br/>

- Delete the entire cloned repo and re-clone. The way the tools are installed means as long as you clone into the same directory as the first time everything should be fine:
```
rm -rf ./BashTools
sudo git clone https://github.com/owenCocjin/BashTools.git
```

In order to update the `update.sh` script itself, you must manually run the below command __IN THE REPO DIRECTORY__:
```
rm ./update.sh
wget -O update.sh https://raw.githubusercontent.com/owenCocjin/BashTools/master/update.sh
chmod +x ./update.sh

```

<br/>

## Usage:

After installing, you can run any of the following as commands:
* cl
	* cd then ls into a directory
* fillSpaces
	* Replaces spaces in filenames
* n
	* Send & dissociate a program from a terminal
* resetWifi
	* Restart a wifi card
* stickynotes
	* Create and manage stickynotes
* wttr
	* Get weather info

<br/>

## Uninstall:

To uninstall you must:

- Manually change the edits made by the install script in your .bashrc file. See install instructions for specific lines.

- Delete the symlink in the bashtools path. Default will be `/usr/local/bin/bashtools`.

- Delete the BashTools cloned repo.
