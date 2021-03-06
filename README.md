fermentrack-tools
============

Various tools to setup/update/configure BrewPi/Fermentrack

* **install.sh** - This is a stand-alone bash script that will install Fermentrack onto a Raspbian distro

* **install-esp8266.sh** - This is a stand-alone bash script that will download the necessary files for setting up an ESP8266 to act as a BrewPi controller into this directory.

* **update-tools-repo.sh** - This is a stand-alone bash script that will update fermentrack-tools to the latest version

* **automated_install/auto-install.sh** - This is a bash script that is intended to be called via `curl -L install.fermentrack.com | sudo bash`

## Automated Fermentrack Installation Instructions

Want to quickly install Fermentrack onto your Raspberry Pi? Installation can now be completed with one easy command:

1. Log into your Raspberry Pi via SSH (or bring up the terminal)
2. Run `curl -L install.fermentrack.com | sudo bash`
3. Done!

## Manual Fermentrack Installation Instructions

Prefer to install everything manually? No problem. Just run the following and you'll be up and running quickly:

1. Log into your Raspberry Pi via SSH (or bring up the terminal)
2. Run `sudo apt-get update` and 
3. Run `sudo apt-get install -y git-core build-essential python-dev python-virtualenv`
4. Clone the `fermentrack-tools` repo using `git clone`
5. Run `sudo fermentrack-tools/install.sh`
6. Follow the prompts on screen to complete installation
7. Done!


## Note from Thorrak
This script was originally based on the fantastic brewpi-script by Elco/Freeder. Since then, it has been modified to install Fermentrack (instead of brewpi-www and brewpi-script) and utilize scripts in those repos to manage updates.

The automated installer was inspired by the Pi-Hole project. 

**PLEASE NOTE** - Piping anything - especially from a website - to `bash` is dangerous -- and especially so when piping to `sudo bash`. If you feel more comfortable installing things manually, please do so.

