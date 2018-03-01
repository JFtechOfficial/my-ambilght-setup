[![banner](https://dl.dropboxusercontent.com/s/xbczn9daprt7q2i/banner.png?dl=0 "banner with JFtech logo & social")](https://linktr.ee/jftechofficial)
[![Raspberry Pi](https://img.shields.io/badge/made%20for-Raspberry%20Pi-red.svg)](https://www.raspberrypi.org) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com) ![license](https://img.shields.io/github/license/JFtechOfficial/ultimate-ambilght-setup.svg) ![GitHub issues](https://img.shields.io/github/issues/JFtechOfficial/ultimate-ambilght-setup.svg) ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/JFtechOfficial/ultimate-ambilght-setup.svg) ![GitHub top language](https://img.shields.io/github/languages/top/JFtechOfficial/ultimate-ambilght-setup.svg) ![Requires.io](https://img.shields.io/requires/github/JFtechOfficial/ultimate-ambilght-setup.svg)

Scripts I created to enhance the Hyperion experience. You can also read this in [Italian🇮🇹](README-it-IT.md)

## 🚀 Getting started
??? lorem ipsum ???
<details>
 <summary><strong>Table of Contents</strong> (click to expand)</summary>

* [Getting started](#-getting-started)
* [Installation](#-installation)
* [Configuration](#️-configuration)
* [Usage](#️-usage)
* [Examples](#-examples)
* [Resources](#-resources)
* [Notes](#-notes)
* [Troubleshooting & debugging](#-troubleshooting--debugging)
* [Contributing](#-contributing)
* [Credits](#️-credits)
* [License](#-license)
</details>

### Requirements
* A Raspberry Pi 2 or 3
* A microSD card with an OS installed ([OSMC](https://osmc.tv/download/) is suggested)

You can install [hyperion](https://hyperion-project.org) now or after the installation step




## 💾 Installation
```shell
wget https://raw.githubusercontent.com/JFtechOfficial/ultimate-ambilght-setup/master/install.sh
```
(you can modify the install.sh file if you don't want to install all the scripts)

```shell
sudo chmod +x install.sh
sudo ./install.sh
```

## ⚙️ Configuration

### Clock effect
* move both `clock.py` and `clock.json` to the Hyperion effects folder 
```shell
sudo mv clock.* /usr/share/hyperion/effects/
``` (default path)
* [Get your OpenWeatherMap API key](http://openweathermap.org/appid) 
* open the `clock.json` file
```shell
sudo nano clock.json
```
* Paste the key in the `clock.json` file (you can use the same key in the kodi weather app)
* [Get your coordinates](https://support.google.com/maps/answer/18539?co=GENIE.Platform%3DDesktop&hl=en&oco=1) 
* Paste both latitude and longitude in the `clock.json` file
* You can modify the default colors of the "virutal" clock hands and add markers
* Save and close the file
*JFtech needs to insert a GIF here*


### Buttons
* open the `buttons.py` file
```shell
nano buttons.py
```
* modify the `Pins` and `clear` variables to match your GPIO setup
* Save and close the file

### Fan
* open the `fan.py` file
```shell
nano fan.py
```
* modify the `pin` variable to match your GPIO setup
* you can modify the default `max_TEMP` variable (Temperature in Celsius after which the fan triggers),
`cutoff_TEMP` variable (Temerature in Celsius after which the fan stops) and `sleepTime` variable (Temperature reading interval in seconds)
*JFtech needs to insert a GIF here* or you can activate one of the pre-made fan profile by uncommenting it *JFtech needs to insert a GIF here*
* Save and close the file


Remember to reboot your device after the configuration
```shell
sudo reboot
```

## ▶️ Usage

Use your favorite Hyperion client to 

## 💼 Examples


## 📚 Resources


## 🎁 Contributing

Please see [CONTRIBUTING.md](./CONTRIBUTING.md).

## ❤️ Credits

Major dependencies:

* [ShellJS](https://documentup.com/shelljs/shelljs)
* [Inquirer.js](https://github.com/SBoudrias/Inquirer.js)
* [@octokit/rest](https://github.com/octokit/rest.js)

The following programs have been a source of inspiration:


## 🎓 License

[MIT](http://webpro.mit-license.org/)


