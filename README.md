# PROVE - Productivity-Reinforcement-Oriented Voltaic Extension

Are you looking for a way to inspire productivity within your code development? Are the traditional KPIs of your "product manager" uses not providing sufficient motivation to get things done? Maybe PROVE is the motivational mistress you need.

PROVE is a Visual Studio Code extension that enables developers to enhance their coding experience with voltaic stimulation from supported devices.

The extension leverages the PiShock "cloud" api to connect to your device and provide real-time productivity reinforcement as you do note type into your VSCode editor.

## Features

- Connects to your supported voltaic-enabled devices from the PiShock brand.
- Voltaic intensity builds up with **in**consistent typing, reaching a maximum threshold.
- Voltaic intensity decreases over time in response to typing.

## Requirements

- Visual Studio Code (VSCode)
- An account with PiShock and paired voltaic peripherals.

## Installation

1. Open VS Code
2. Go to the Extensions view (`⇧⌘X` on macOS or `Ctrl+Shift+X` on Windows/Linux)
3. Search for `PROVE` and click the Install button
4. Once the installation is complete, click the Reload button

## Usage

1. Connect your supported device to your computer via the Intiface Central software
2. Open Visual Studio Code
3. Run the `PROVE: Connect` command from the Command Palette (`⇧⌘P` on macOS or `Ctrl+Shift+P` on Windows/Linux)
4. Start typing in your VSCode editor to experience the vibration feedback

## Configuration

The following options are available for configuration:

- `prove.serverAddress`: The Intiface Central server address to connect to (typically of the form `ws://SERVER:PORT`)
- `prove.typingWindow`: Length of the gap in typing (in milliseconds) before vibration decreases by a stage
- `prove.vibrationMax`: The maximum vibration intensity that can be achieved
- `prove.vibrationStages`: The number of stages the vibration increases through
  - More stages means a more granular vibration change per stage
  - A higher number will mean more stages to get through to get to maximum vibration
- `prove.vibrationStageLength`: Duration (in milliseconds) of each stage of vibration
  - Longer stage length will mean a longer ramp up time to get to maximum vibration

## Support

For any issues or questions, please visit the [PROVE GitHub repository](https://github.com/drawnto/prove).

## The Future Of PROVE

Note that all of the below listed ideas are merely concepts - there are no guarantees or roadmap.

- "Panic Button" keybind to disconnect
- Event-triggered interactions
  - On save
  - When running tests
- Automatically refresh device list
- Connect on load (toggleable)
