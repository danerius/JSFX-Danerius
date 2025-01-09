
# Last Samples High Cut

## Overview
A lightweight JSFX plugin that implements a simple but effective lowpass filter. The plugin works by averaging the current sample with the previous sample, with an adjustable blend ratio. Great for taming harsh high frequencies and adding a warm, vintagey feel to your audio.

## Parameters
- **High Cut** (0.5 - 1.0): Controls the mix between the current and previous sample. 
  - At 0.5: Equal mix between current and previous sample
  - At 1.0: Maximum filtering effect (more previous sample)

## Technical Details
The plugin processes left and right channels independently. For each channel:
1. Stores the current sample
2. Calculates weighted average between current and previous sample
3. Updates previous sample memory
4. Outputs the processed result

## Installation
1. Place the plugin file in your REAPER JSFX directory
2. Refresh your JSFX list in REAPER
3. The plugin will appear as "Last Samples High Cut (Danerius)"

## Usage
Once installed, you can access the Last Samples High Cut plugin from your audio host's effects menu. The plugin comes with a default preset that can be customized to suit your needs.

## Configuration
The default settings can be found in the `src/presets/default.jsfx-preset` file. You can modify these settings to create your own presets.

## Examples
For usage examples and detailed instructions, refer to the documentation in the `doc` directory.

## Contributing
If you would like to contribute to the Last Samples High Cut plugin, please fork the repository and submit a pull request with your changes.
