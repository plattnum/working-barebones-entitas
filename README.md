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


