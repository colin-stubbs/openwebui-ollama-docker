# MacOS launchtl Service

## Regular User

The ollama.plist file should be installed to ~/Library/LaunchAgents/ollama.plist

Modify the environment variables list via EnvironmentVariables XML node as required.

The example for `OLLAMA_HOST` is prefixed with `DISABLED_` as an example for how to disable use of an environment variable without deleting it from the .plist file. 

NOTE: You will need to launchctl stop/unload/load/start the service again to get any changes to be implemented.
NOTE: You may need to create ~/Library/LaunchAgents via `mkdir -p ~/Library/LaunchAgents/` first.

As your regular user run the following to start the service,
```
launchctl load -w ~/Library/LaunchAgents/ollama.plist
launchctl start ollama
```

Example,
```
TBC
```

