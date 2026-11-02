![Motobox banner](https://cdn.modrinth.com/data/mw9W1jZT/images/cfaf398e31b35a2c40ada3024049f260ea945216.png)

![](https://img.shields.io/badge/Mod_Loader-Fabric-6a6a6a?style=for-the-badge&labelColor=272727)
[![](https://img.shields.io/badge/-Github-6a6a6a?style=for-the-badge&labelColor=272727&logo=github)](https://github.com/Project-Alphaa/Motobox)
[![](https://img.shields.io/badge/-Curseforge-6a6a6a?style=for-the-badge&labelColor=272727&logo=curseforge)](https://www.curseforge.com/minecraft/mc-mods/motobox)
[![](https://img.shields.io/badge/-Modrinth-6a6a6a?style=for-the-badge&labelColor=272727&logo=modrinth)](https://modrinth.com/mod/motobox)
[![](https://img.shields.io/badge/Discord-6a6a6a?style=for-the-badge&labelColor=272727&logo=discord)](https://discord.gg/the-alpha-server-852655613669277777)

### **Building**
This branch targets Minecraft 1.20.1 with Fabric. Install a JDK 17 and make sure `JAVA_HOME` points to it before building. The checked-in Gradle 8.3 wrapper does not support running on Java 21.

In PowerShell, you can select JDK 17 for the current terminal without changing your system-wide Java installation (replace the example path with your installed JDK):

```powershell
$env:JAVA_HOME = 'C:\path\to\jdk-17'
.\gradlew.bat clean build
```

On Windows, run `.\gradlew.bat build` from the repository root. On macOS or Linux, run `./gradlew build`. The finished mod JAR is written to `build/libs/`.

### **Installing**
Use Fabric Loader for Minecraft 1.20.1. Put the built Motobox JAR and these dependencies in the same game instance's `mods` folder:

- [Fabric API](https://modrinth.com/mod/fabric-api): a Minecraft 1.20.1 release (the build uses 0.91.0+1.20.1).
- [Fabric Language Kotlin](https://modrinth.com/mod/fabric-language-kotlin): the build uses 1.10.17+kotlin.1.9.22.
- [GeckoLib](https://modrinth.com/mod/geckolib): the Fabric release for Minecraft 1.20.1 (the build uses 4.4.2).

These dependencies are available to Gradle during development but are not bundled in the built Motobox JAR. Download their mod JARs separately. Do not use Forge or NeoForge releases.

### **📘 Description**
With Motobox Vehicle Mod, you can customize your vehicles with a variety of wheels, and engines. The mod adds more than three vehicles, including powered vehicles and a useful trailer, for practical use. You can explore, transport, and race with these vehicles. Modify each vehicle with unique engines and wheels to adjust their speed and adaptability to different terrains. The mod also supports controllers with MidnightControls, which allows you to drive the vehicles using a controller.

**Note:** This is a fork of [Automobility](https://modrinth.com/mod/automobility) with our own spin on things, we had permission to do it.
![](https://i.imgur.com/j8YAnhl.png)

### **📚 FAQ**
**Q:** Can I use this mod in my modpack?
<br>
**A:** Yes, feel free to use this mod in your modpack.
<br><br>
**Q:** What are the different game versions that this mod will support?
<br>
**A:** This branch targets Minecraft 1.20.1.

![](https://i.imgur.com/j8YAnhl.png)

🛠 Contributing
If anyone would like to add the remaining features to the game, feel free to check out the Trello board: [Mod Trello Board](https://trello.com/b/BmcUb06n/project-slenderman-main). Just make sure to contact me through my discord server for any help.

![](https://i.imgur.com/j8YAnhl.png)

### **🙎‍♂️ Additional Credits**
- Foundation games (Former Author)
- ~~Qboi~~ XyperCode (Author)
- MincraftEinstein (Contributor)
- Jab125 (Contributor)
- Chumasay (Artist)
- Skylandia (Contributor)
- SJKZ1-2565 (Contributor)
- C0D3_M4513R (Contributor)
