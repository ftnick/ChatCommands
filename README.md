# ChatCommands

ChatCommands is a powerful Roblox script designed to enhance chat functionalities in your game. It provides various commands for managing players, sending notifications, and customizing chat interactions.

## Table of Contents

- [Installation](#installation)
- [Modules](#modules)
  - [CommandsModule](#commandsmodule)
  - [NotificationModule](#notificationmodule)
  - [SystemChatModule](#systemchatmodule)
  - [SettingsModule](#settingsmodule)
- [Usage](#usage)
- [Command List](#command-list)
- [Contributing](#contributing)
- [License](#license)

## Installation

1. **Download** the ChatCommands script.
2. **Place** the `ChatCommands` folder into `ServerScriptService` in your Roblox Studio project. 
3. Ensure that all submodules (`CommandsModule`, `NotificationModule`, `SystemChatModule`, and `SettingsModule`) are correctly parented under `ChatCommands`.

   The structure should look like this:
   ```
   ServerScriptService
   └── ChatCommands
       ├── CommandsModule
       │   ├── LevenshteinDistanceAlgorithm
       ├── NotificationModule
       │   └── MainModule
       ├── SettingsModule
       └── SystemChatModule
           └── LocalScript (Disabled)
   ```

## Modules

### CommandsModule

Handles command processing logic. Includes predefined commands for player management.

### NotificationModule

Manages notification functionalities for players. It utilizes the main notification system to send alerts and messages.

### SystemChatModule

Facilitates the sending of system messages to players. This module manages how messages are displayed in the game chat.

### SettingsModule

Configures various settings, including chat customization and command prefixes.

## Usage

To use the ChatCommands script, players must type commands into the chat box prefixed by the defined command prefix (default: `/`). 

### Example:

To kick a player, type:
```
/kick PlayerName Reason
```

Ensure that the player has the necessary permissions to execute commands.

## Command List

| Command    | Usage                                     | Description                           |
|------------|-------------------------------------------|---------------------------------------|
| `kick`     | `/kick <(Partial)PlayerName> <(Optional)Reason>` | Kicks a player from the server.      |
| `reload`   | `/reload <(Partial)PlayerName>`          | Reloads a player's character.         |
| `tpto`     | `/tpto <(Partial)PlayerName>`            | Teleports you to a player's character.|
| `bring`    | `/bring <(Partial)PlayerName>`           | Brings a player to you.              |
| `announce` | `/announce <Message>`                     | Sends a global announcement.          |
| `cmds`     | `/cmds`                                   | Displays all available commands.      |
| `help`     | `/help <CommandName>`                     | Displays usage and description of a specific command. |

## Contributing

If you wish to contribute to this project, feel free to create a fork and submit a pull request. Any suggestions or improvements are welcome.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

### Author

Made by @repostnick
