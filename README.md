# windows-terminal-vscode
VS Code theme for Windows Terminal

# How to install

Start Windows Terminal and click on the down arrow symbol from menu bar. This will open a drop down menu from which select the Settings option. In the `profile.json` settings file for Windows Terminal, find the `schemes` section and paste the contents of `vs-code.json`:

```json
{
    "name": "VS Code",
    "background": "#21252b",
    "foreground": "#a9b2c3",
    "black": "#21252b",
    "blue": "#61afef",
    "brightBlack": "#5f6672",
    "brightBlue": "#007fff",
    "brightCyan": "#08e8de",
    "brightGreen": "#66ff00",
    "brightPurple": "#8b00ff",
    "brightRed": "#d74e42",
    "brightWhite": "#d4d7d9",
    "brightYellow": "#e5c07b",
    "cyan": "#56b6c2",
    "green": "#98c379",
    "purple": "#b57edc",
    "red": "#e06c75",
    "white": "#a9b2c3",
    "yellow": "#d19a66"
}
```

Once the color scheme has been defined, find the profiles section and add a `colorScheme` value to the default profile:

```json
    "profiles":
    {
        "defaults":
        {
            "colorScheme": "VS Code"
        },

    }
```

![Image description](https://github.com/cristipufu/windows-terminal-vscode-theme/blob/master/windows-terminal-vs-code-theme.JPG)

## Bonus

If you also want to change your key bindings (copy-paste & browser-like tabbing), find the `keybindings` section and update it for your needs:

```json
    "keybindings": [{
        "command" : "closeTab",
        "keys" :[
            "ctrl+w"
        ]
    },
    {
        "command" : "newTab",
        "keys" :[
            "ctrl+t"
        ]
    },
    {
        "command" : "copy",
        "keys" :[
            "ctrl+c"
        ]
    },
    {
        "command" : "paste",
        "keys" : [
            "ctrl+v"
        ]
    }]
```


