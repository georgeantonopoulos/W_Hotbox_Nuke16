# W_hotbox for Nuke 16

This is a modified version of Wouter Gilsing's W_hotbox for Nuke, updated to work with Nuke 16.

## Features

W_hotbox is a powerful, fully customizable button interface that appears on hotkey press in the Node Graph. It allows for:

- Quick access to frequently used nodes and node operations
- Contextual functionality based on selected node types
- Custom scripts and actions accessible via simple buttons
- User-defined organization and color coding
- Shareable button collections

## Nuke 16 Compatibility

This fork has been specifically updated to be compatible with Nuke 16, which uses Python 3.11 and PySide6 instead of PySide2 as in previous Nuke versions. Key changes include:

- Updated Qt import system that detects and prioritizes PySide6 for Nuke 16
- Maintains backward compatibility with older Nuke versions (11-15 use PySide2, 10 and earlier use PySide)
- Improved error messaging for import issues

## Installation

1. Copy `W_hotbox.py` and `W_hotboxManager.py` to a folder in your Nuke plugin path (usually inside `~/.nuke`)
  
2. Append your `menu.py` with:
   ```python
   import W_hotbox, W_hotboxManager
   ```

3. Copy the `icons` folder to your `.nuke` folder, or set a custom path in the W_hotbox preferences

4. Launch Nuke and access the hotbox using the backtick key (`) by default

For detailed installation instructions, see the `InstallationGuide.txt` file.

## Usage

- Press the hotkey (default: `) to show the hotbox
- Select a button to execute its associated function
- Access the Hotbox Manager from the Edit menu or from within the hotbox to create, edit, and organize your buttons

## License

This project is licensed under the BSD 3-Clause License - see the LICENSE file for details. The original work was created by Wouter Gilsing, and this repository contains modifications for Nuke 16 compatibility by George Antonopoulos. 
