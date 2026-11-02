![68747470733a2f2f63646e2e6d6f6472696e74682e636f6d2f646174612f6d773957316a5a542f696d616765732f636661663339386533316233356132633430616461333032343034396632363065613934353231362e706e67](https://github.com/user-attachments/assets/99d4e457-d03d-445a-b510-82220d13166a)

![](https://img.shields.io/badge/Mod_Loader-Fabric-6a6a6a?style=for-the-badge&labelColor=272727)
[![](https://img.shields.io/badge/-Github-6a6a6a?style=for-the-badge&labelColor=272727&logo=github)](https://github.com/Project-Alphaa/Motobox)
[![](https://img.shields.io/badge/-Curseforge-6a6a6a?style=for-the-badge&labelColor=272727&logo=curseforge)](https://www.curseforge.com/minecraft/mc-mods/motobox)
[![](https://img.shields.io/badge/-Modrinth-6a6a6a?style=for-the-badge&labelColor=272727&logo=modrinth)](https://modrinth.com/mod/motobox)
[![](https://img.shields.io/badge/Discord-6a6a6a?style=for-the-badge&labelColor=272727&logo=discord)](https://discord.gg/rtEGCzbZym)

### **Building**
This branch targets Minecraft 1.20.1 with Fabric. Install a JDK 17 and make sure `JAVA_HOME` points to it before building. The checked-in Gradle 8.3 wrapper does not support running on Java 21.

In PowerShell, you can select JDK 17 for the current terminal without changing your system-wide Java installation (replace the example path with your installed JDK):

```powershell
$env:JAVA_HOME = 'C:\path\to\jdk-17'
.\gradlew.bat clean build
```

On Windows, run `.\gradlew.bat build` from the repository root. On macOS or Linux, run `./gradlew build`. The finished mod JAR is written to `build/libs/`.

Kotlin compiles inside Gradle's JVM to avoid reusing an IDE-started Kotlin daemon running on an incompatible Java version (such as Java 25). The Gradle JVM must still use JDK 17; the Java/Kotlin bytecode target does not select the JVM running the build.

For VS Code's Java project import, set `java.import.gradle.java.home` to your JDK 17 installation in local workspace settings. For Gradle extension tasks, set `gradle.java.home` there too. Do not change `java.jdt.ls.java.home`: the Java language server can use its bundled newer JDK independently.

If Gradle still selects a different JVM, pass `"-Dorg.gradle.java.home=$env:JAVA_HOME"` to the wrapper after setting `JAVA_HOME` to JDK 17.

VS Code's Java language server cannot read Kotlin source directly. The Gradle Eclipse model adds compiled Kotlin classes to its classpath and compiles them during project synchronization. After changing Kotlin models, run `.\gradlew.bat compileKotlin` and **Java: Reload Projects**. If unresolved Kotlin imports persist, run **Java: Clean Java Language Server Workspace** and allow the project to reimport. Java imports use the class's package/name regardless of whether its source is `.java` or `.kt`.

### **Installing**
Use Fabric Loader for Minecraft 1.20.1. Put the built Motobox JAR and these dependencies in the same game instance's `mods` folder:

- [Fabric API](https://modrinth.com/mod/fabric-api): a Minecraft 1.20.1 release (the build uses 0.91.0+1.20.1).
- [Fabric Language Kotlin](https://modrinth.com/mod/fabric-language-kotlin): the build uses 1.10.17+kotlin.1.9.22.
- [GeckoLib](https://modrinth.com/mod/geckolib): the Fabric release for Minecraft 1.20.1 (the build uses 4.4.2).

These dependencies are available to Gradle during development but are not bundled in the built Motobox JAR. Download their mod JARs separately. Do not use Forge or NeoForge releases.

### **📘 Description**
Experience a driving simulator where you can fully customize your vehicles, including powered options and a useful trailer, with a range of wheels and engines for practical use. Explore, transport, and race with these vehicles, each modifiable to enhance speed and adaptability to various terrains. This mod also supports controllers via MidnightControls, allowing you to drive with ease using a controller.

**Note:** This is a fork of [Automobility](https://modrinth.com/mod/automobility) with our own spin on things, we had permission to do it.
![](https://i.imgur.com/j8YAnhl.png)

### **📚 FAQ**
**Q:** Can I use this mod in my modpack?
<br>
**A:** Yes, feel free to use this mod in your modpack.
<br><br>
**Q:** I have an inquiry about something. Can you help?
<br>
**A:** This fork is maintained by a different developer than those who run the Discord. Ask away in the comments, or on the Discord server, but again - the Discord is not run by the developer of this fork!

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
