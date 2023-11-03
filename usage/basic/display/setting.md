# Setting

### classic

output like ls, without color and icon

`--classic`

### colorless

disable color

`--colorless` or `--no-color`

### theme

`g` uses JSON file to configure custom theme

The colors listed below are supported

```
Black       
Red         
Green       
Yellow      
Blue        
Purple      
Cyan        
White       
BrightBlack 
BrightRed   
BrightGreen 
BrightYellow
BrightBlue  
BrightPurple
BrightCyan  
BrightWhite 
```

and 256 color should be the form of `[code]@256`

true color/ 24bit color should be the form of `[r,g,b]@rgb`

hex form: `[str]@hex`

#### example

{% code title="custom-theme" %}
```json
{
    "info": {
        "-": {
            "color": "white"
        },
        "inode": {
            "color": "purple"
        },
        "reset": {
            "color": "reset"
        },
        "time": {
            "color": "blue"
        }
    },
    "permission": {
        "-": {
            "color": "white"
        },
        "D": {
            "color": "cyan"
        },
        "b": {
            "color": "yellow"
        },
        "c": {
            "color": "yellow"
        },
        "d": {
            "color": "blue"
        },
        "l": {
            "color": "purple"
        },
        "octal": {
            "color": "[208]@256"
        },
        "p": {
            "color": "yellow"
        },
        "r": {
            "color": "yellow"
        },
        "s": {
            "color": "yellow"
        },
        "w": {
            "color": "red"
        },
        "x": {
            "color": "green"
        }
    },
    ...
```
{% endcode %}

```json
"readme": {
            "color": "yellow",
            "icon": "<U+F48A>",
            "underline": true,
            "bold": true,
            "faint": false,
            "italics": false,
            "blink": false
},
```

full theme : [\[default\]](https://github.com/Equationzhao/g/blob/master/theme/default.json)

#### apply theme

```bash
g --theme=path-to-theme-file
```
