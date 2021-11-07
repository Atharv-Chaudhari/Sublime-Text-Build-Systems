# Sublime-Text-Build-Systems

### For Python Build :- 

#### Normal Python Build System with CMD
```bash
{
    "cmd": ["start", "cmd", "/C", "py -u $file_name", "& echo. & pause"],
    "file_regex": "^[ ]*File \"(...*?)\", line ([0-9]*)",
    "selector": "source.python",
    "shell": "true",
}
```
