# Disclaimer

Please note that this repository is no longer being actively maintained or updated. 
After further evaluation, I found a better solution to my needs by using the [SMARTLIGHT SLWF-01pro](https://smartlight.me/smart-home-devices/wifi-devices/wifi-dongle-air-conditioners-midea-idea-electrolux-for-home-assistant). 
This product offers the functionality I require and aligns more closely with my goals for future projects.

Feel free to explore the code and use it as you see fit, but be aware that no further development or support will be provided.

Thank you for your understanding, and if you need any help please feel free to reach out!



# Commands for Vulcano Air Conditioner (Line Cool) through MOES Universal Remote Control (UFO-R11) 

Welcome to the Vulcano AC Line Cool IR project! This repository contains a collection of commands for controlling your Vulcano Air Conditioner from the Line Cool series using the MOES UFO-R11 universal remote control. Please note that this project is a work in progress, and we encourage contributions from the community to expand its capabilities.

## Project Status

**Status: Work in Progress**

This project is actively being developed to document and expand the list of available commands for controlling the Vulcano Line Cool Air Conditioner. While the existing commands should be functional, there may be additional features and improvements to come.

## Getting Started

To use the MOES Universal Remote Control (UFO-R11) commands for your Vulcano Line Cool Air Conditioner, follow these steps:

1. **Clone the Repository:**
   ```
   git clone https://github.com/davidrpfarinha/Vulcano-AC-Line-Cool-IR-Commands.git
   ```

2. **Navigate to the Repository:**
   ```
   cd vulcano-ac-line-cool-ir-commands
   ```

3. **Review the Commands:**
   Browse the repository to find the list of available commands in the [AC Vulcano IR Commands](https://github.com/davidrpfarinha/Vulcano-AC-Line-Cool-IR-Commands/blob/main/4209.json) file. This file provides a detailed list of commands and their functions.

4. **Use the Commands:**
   Use the commands in your MOES UFO-R11 remote control to control your Vulcano Line Cool Air Conditioner.

## Contributing

We welcome contributions from the community to improve this project. If you have discovered new commands, found ways to optimize existing ones, or have suggestions for enhancements, please consider contributing. To contribute, follow these steps:

1. **Fork the Repository:**
   Click the "Fork" button at the top right of the repository to create a copy of it in your GitHub account.

2. **Clone Your Fork:**
   ```
   git clone https://github.com/davidrpfarinha/Vulcano-AC-Line-Cool-IR-Commands.git
   ```

3. **Create a New Branch:**
   ```
   git checkout -b feature/new-command
   ```

4. **Make Changes:**
   Add, modify, or delete commands as needed.

5. **Commit Your Changes:**
   ```
   git commit -m "Added a new command for [Function]"
   ```

6. **Push to Your Fork:**
   ```
   git push origin feature/new-command
   ```

7. **Create a Pull Request:**
   Go to your fork on GitHub, and click the "New Pull Request" button. Explain your changes and submit the pull request.

## How I'm using it

I've incorporated these IR commands into my Home Assistant setup, allowing me to transmit them using an IR blaster. 
To enable this functionality, I had to introduce specific [quirks](https://github.com/zigpy/zha-device-handlers/issues/1687#issuecomment-1424357574) to facilitate the learning and transmission of these commands. 
With these quirks in place, I can now efficiently teach my IR blaster these codes and issue them directly from my Home Assistant environment.

## Update

I've installed the [SmartIR](https://github.com/smartHomeHub/SmartIR/) component, and created a new file called 4209.json to host the commands.
Then, I customized the SmartIR integration to be able to call the services exposed by the abovementioned quirks.
With this, I now have an climate entity that can be used natively.

Kudos to [@ferehcarb](https://github.com/ferehcarb) for the development of the quirk, and to [@smartHomeHub](https://github.com/smartHomeHub/SmartIR) for their custom integration.

## Contact

If you have questions or need assistance, feel free to contact the project maintainers through GitHub issues.

Enjoy controlling your Vulcano Line Cool Air Conditioner with your MOES UFO-R11 remote control! Thank you for contributing to this project's development.
