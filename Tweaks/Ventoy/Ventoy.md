# Ventoy

### First install ventoy 

```
https://www.ventoy.net/en/download.html
```

### To edit the ventoy Grup tweaks 

```
gnome-look.org  ## themes 
```

### To add the Grup 

- create a "ventoy" folder in pendrive
- create a "themes" folder inside ventoy folder
- create a "ventoy.json" file inside ventoy folder
  
```
### https://www.ventoy.net/en/plugin_entry.html
{
    "theme": {
       "file": "/ventoy/theme/"Folder PATH"/theme.txt"
   }
}
```
- or
  
 ```
{
    "control": [
        { "VTOY_DEFAULT_MENU_MODE": "1" },
        { "VTOY_FILT_DOT_UNDERSCORE_FILE": "1" }
    ],
    
    "theme": {
        "file": "/ventoy/theme/"Folder PATH"/theme.txt",
        "gfxmode": "1920x1080"
    }
}
 ```
