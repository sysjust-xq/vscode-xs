# README

Visual Studio Code extension providing syntax highlighting for [XS script language](https://www.xq.com.tw/School.aspx).

![DarkTheme](https://raw.githubusercontent.com/sysjust-xq/vscode-xs/master/images/dark.png)

![LightTheme](https://raw.githubusercontent.com/sysjust-xq/vscode-xs/master/images/light.png)

## Installation

You can install this extension from [VSCode Marketplace](https://marketplace.visualstudio.com/items?itemName=sysjust-xq.xs).

Or you can install manually by copying everything inside xs subfolder to <HomeDirectory>\.vscode\.extensions\xs:

```
C> xcopy /E/H vscode-xs\xs %userprofile%\.vscode\extensions\xs\ 
```

## Customization

The color of syntax highlighting depends on the themes you have selected.

If you want to perform further customization, add an "editor.tokenColorCustomizations" section to your vscode `settings.json`. The following example will change the color of operator to RED:

```json

    "editor.tokenColorCustomizations" : {
        "textMateRules": [
            {
                "scope": "keyword.operator",
                "settings": {
                    "foreground": "#FF0000"
                }
            }
        ]
    }
```

Please see [VS Code document](https://code.visualstudio.com/docs/getstarted/themes) for more information.

These are the token scopes that you can customize:

- variable.builtin.xs (內建變數, 例如 value1, value2)
- variable.field.xs (內建欄位, 例如 open, high)
- variable.constant.cs (內建常數, 例如 PI)
- keyword.control.xs (內建流程關鍵字, 例如 if, then)
- keyword.operator.xs (內建運算字元, 例如 +, -, *)
- keyword.bif.xs (內建函數, 例如 CurrentBar, CurrentTime)
- keyword.sysfnc.xs (系統函數, 例如Average, Summation)


## License

[MIT](https://raw.githubusercontent.com/derektu/vscode-xs/master/LICENSE)

        