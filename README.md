# Unity OpenTerminal

## Installation
You can install this package via git url by adding this entry into your manifest.json file
```
"io.redstart.open-terminal": "https://github.com/redstartinteractive/OpenTerminal.git#upm"
```

## Features

- Add cheat codes to your game.
- Enable GOD MODE while testing your code.
- Shows return type of a command in terminal
- Custom Terminal configs.
- AutoComplete: press tab and see available commands. thanks to [@kenculate](https://github.com/kenculate)
- Report your game log to an email address(useful for testers)
- Mobile input support

![open-terminal](https://user-images.githubusercontent.com/6388730/84697557-9be01b00-af63-11ea-9971-e3e4dd3922c3.gif)

## How to use

- Add [TerminalCommand("commandName", "commandDescription")] Attribute to public MonoBehaviour methods.
- Create an empty game object and add Terminal component to it.
- Run your game and press ` (tilde) to show the terminal. 
- On mobile long press with 4 fingers to show terminal.
- Type your commandName and it will execute!

## Code usage

Simple usage:

```csharp
    [TerminalCommand("rotate-cube", "rotates the cube")]
    public void RotateTheCube()
    {
        stop = false;
    }
```

With parameters:

```csharp
    [TerminalCommand("move-cube", "move-cube(x,y,z) Moves the cube")]
    public void Move(float x, float y, float z)
    {
        transform.position = new Vector3(x, y, z);
    }
```

## Change theme

Edit config file to change fonts and colors

![image](https://user-images.githubusercontent.com/6388730/27377905-8dd0b4b8-568b-11e7-83f0-775d943773a9.png)

## Limitations

- Does not support vectors or other parameters which contain "," as method input.

## Deploy new version
You can deploy a new version of the package to the repository by running the script `deploy.sh`

## License

[MIT License](LICENSE)
