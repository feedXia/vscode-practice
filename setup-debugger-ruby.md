# How to Setup Debugger in VS Code for Ruby

_Disclaimer: I'm using a 2020 M1 MacBook Air, running on Mac OS Big Sur ver 11.3.1, and VS Code_ver 1.60.1 (Universal).

1. Download the Ruby Extension in VS Code: (Extension ID: rebornix.ruby)
2. If you don't yet have a "launch.json" file, create one: [Link to creating the "launch.json" file!](https://code.visualstudio.com/docs/editor/debugging)
3. In "launch.json": add the configuration named "Listen for rdebug-ide"
4. Edit the configuration so it looks like this:
5. Add another configuration for running your local Ruby files like this:

## Entering Inputs While Debugging (Ongoing)

Currently there seems to be no know mehtod built into VS code that allows you to provide input when debugging files that require user input (e.g. files that contain "gets.chomp").

One possible work around I've found is [this!](https://github.com/microsoft/vscode-cpptools/issues/5079#issuecomment-626090192) , but so far it seems to launch a separate console underneeth the debugger but does not act on any input provided.
