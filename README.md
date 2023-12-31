# Polyfact Extension

## Overview

The VSCode extension can help you add references to your code. Press CMD + SHIFT + D; the extension will create function references and insert them as comments in your code. The extension uses the Polyfact API to generate the references.

## Current Version

As of the latest update, the project is at version 0.1.2

## License

The Polyfact Extension is open-source software licensed under the terms of the MIT license, promoting reuse and further development by the coding community.

## Key Features

- **Command Activation**: The `polyfact-extension.commentFunctions` command, once executed, activates the extension.
- **Accessible Keybindings**: To invoke the command, use the keyboard shortcut `Ctrl+Shift+D` (`Cmd+Shift+D` on macOS) when the text editor is focused.
- **Context Menu Activation**: Users can also activate the Polyfact Extension by right-clicking in the editor and selecting 'Polyfact Extension' from the context menu.
- **Comment Detail Level Selection**: The extension now offers a configurable 'Mode' setting to choose the level of detail in the generated block comments. Users can select between 'light', 'normal', and 'reinforced' modes, each offering different levels of comment detail.

## Configuration and Access Token Acquisition

To set the detail level for the generated comments:

1. Navigate to the Visual Studio Code settings (File > Preferences > Settings).
2. In the search bar at the top of the settings panel, type 'Polyfact Extension'.
3. Click on 'Edit in settings.json' under the 'Polyfact Extension' section.
4. In the settings.json file, add a new line within the JSON object: `"polyfact-extension.mode": "<your_preferred_mode>"`
5. Replace `<your_preferred_mode>` with either 'light', 'normal', or 'detailed'.
6. Save the settings.json file to apply the changes.

The Polyfact Extension requires an access token for integration with the Polyfact API. Here's how to acquire an access token and configure the `polyfact-extension.accessToken`:

1. Visit [Polyfact's application](https://app.polyfact.com/) and click on 'Connect with Github'.
2. Once you're authenticated with Github, you will be able to see your access token.
3. Copy the provided access token.
4. Now, navigate to the Visual Studio Code settings (File > Preferences > Settings).
5. In the search bar at the top of the settings panel, type 'Polyfact Extension'.
6. Click on 'Edit in settings.json' under the 'Polyfact Extension' section.
7. In the settings.json file, add a new line within the JSON object: `"polyfact-extension.accessToken": "<your_access_token>"`
8. Replace `<your_access_token>` with the access token you copied from the Polyfact application.
9. Save the settings.json file to apply the changes.

## Repository

The source code for the Polyfact Extension is publicly accessible via [this GitHub repository](https://github.com/polyfact/polyfact-extension.git). We welcome contributors and users alike to explore the codebase, report issues, or even propose enhancements.

## Compatibility

The Polyfact Extension is compatible with Visual Studio Code version 1.79.0 or higher, ensuring it can seamlessly integrate with your existing development environment.

## Category

The Polyfact Extension falls under the "Other" category in Visual Studio Code extensions.
