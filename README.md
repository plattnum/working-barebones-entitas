# My Rough Setup Notes For 1.14.1

- Only setup and tested with dotnet Jenny/Jenny.Generator.Cli.dll commands.

1. Downloaded the Entitas release 1.14.1 Entitas.zip and Jenny.zip.
Unzipped Entitas, Removed the internal Jenny folder, moved the Entitas folder to my Unity Assets directroy.

2. Unzipped the Jenny.zip and placed at the root of my Unity project. (1 Level Above Assets)

3. Used this Jenny.properties to get started: https://github.com/sschmid/Match-One/blob/main/Jenny.properties

4. Copied over Jenny-AutoImport, Jenny-Auto-Import.bat, Jenny-Server and Jenny-Server.bat from same github. (Didn't end up using them, I ran into trouble with them.)

5. Updated the Jenny.SearchPath to lookd at Assets/Entitas/Entitas.


6. Using just terminal from root of unity project


- \working-barebones-entitas\unity-entitas> dotnet Jenny/Jenny.Generator.Cli.dll gen
- \working-barebones-entitas\unity-entitas> dotnet Jenny/Jenny.Generator.Cli.dll help

-v really helped. :)


usage:

  help                         Show help
  wiz                          Setup Jenny, guided by a wizard

Code Generation:

  client [command]             Start client mode
  dry                          Run the code generator in dry mode
  gen                          Generate files based on properties file
  server                       Start server mode

Plugins:

  auto-import                  Find and import all plugins
  doctor                       Check the config for potential problems
  fix                          Add missing keys and add available or remove unavailable plugins interactively
  scan                         Scan and print available types found in specified plugins
  status                       List available and unavailable plugins

Properties:

  add [key] [value]            Add a value to a key
  dump                         List all config keys and values
  edit                         Open config files with default editor
  format [-mini]               Format the config files
  new [file] [userFile] [-f]   Create new properties file(s) with default values
  remove [key] [value]         Remove a key or a value from a key

[-v]                         - verbose output
[-s]                         - silent (minimal output)

Menus

  Down, Right, j, l          - Select next
  Up, Left, k, h             - Select previous
  Home, a                    - Select first
  End, e                     - Select last
  Enter, Space               - Run selected menu entry
