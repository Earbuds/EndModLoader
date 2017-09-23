<p align="center"> 
    <img src="https://i.imgur.com/quyR8Am.png" alt="Screenshot of the MOD loader">
</p>

### Download HERE:
[🤖 v1.1 w/ EXE Editing (latest)](https://github.com/Earbuds/EndModLoader/releases/download/v1.1-exe/EndModLoader.exe)
[😼 v1.1](https://github.com/portal-chan/EndModLoader/releases/download/v1.1/EndModLoader.exe)
[🍉 v1.0](https://github.com/portal-chan/EndModLoader/releases/download/v1.0/EndModLoader.exe)   

### For players:
Once you launch the program, assuming you have a Steam version of the game, the program will
automatically initialize a `mods` folder in your games directory. Otherwise, click the "Select"
button and navigate to your directory of choice.

After that's done, put any and all mod .zip files into the `mods` folder. They should automatically
be detected by the program, however if they don't show up, try relaunching.

In specific circumstances, symbols may appear in the same area of the mod.

An **E** with a red background means the mod changes the EXE in some way. 
Don't worry, the program minimizes the risk of anything going wrong!

A **S** with a pink background means the mod supplies its own custom SWF.
Be on the lookout for things you won't be able to find in any other mod!

To launch a mod, select it in the list and click the "Play MOD" button (shoutout to teamPROBIRTH)
and your game will launch running the mod. Once you exit the game, the mod files are cleaned up and
your game is back to normal.

### For modders:
Compress 🗜️ all of your modified unpacked folders into a single .zip file.
In addition, you can include a `meta.xml` file in the root of the .zip file following the example below.
If no `meta.xml` is present, the title defaults to the name of the .zip file and no author/version is displayed.
```xml
<mod>
    <title>Your mod title</title>
    <desc>Short mod info/description</desc>
    <author>Your name</author>
    <version>v1.0</version>
</mod>
```

With the newest version, you are also allowed to make edits to the EXE from inside of your mod!
To do this, include a file called `exepatch.xml` in the root of the .zip file alongside your `meta.xml`.
In order to use it correctly, format it as so:
```xml
<mod>
    <entry>0022DD26~35</entry>
</mod>
```

In this example, the number before the ~ is the hexidecimal address of the value you wish to change
and the number after the ~ is the hexidecimal value you wish to change the address to.

This feature is still experimental and might need a bit of trial and error to guarantee a working mod.

With that your .zip file is ready to be distributed and shilled freely.
