# ✨ Sublime-Text-Build-Systems ✨

### 📋 For Python Build :- 

#### 🧿 Normal Python Build System with CMD

```bash
{
    "cmd": ["start", "cmd", "/C", "py -u $file_name", "& echo. & pause"],
    "file_regex": "^[ ]*File \"(...*?)\", line ([0-9]*)",
    "selector": "source.python",
    "shell": "true",
}
```

#### 🧿 Generalised Python Build System with Spaces in file name runs on cmd

```bash
{
    "shell_cmd": "start cmd /C \"(py -u \"$file\" || set /p = Failed execution. Press Enter to exit...) && set /p = Successful execution. Press Enter to exit...\"",
    "file_regex": "^[ ]*File \"(...*?)\", line ([0-9]*)",
    "selector": "source.python",
    "shell": "true",
}
```

#### 🧿 Path Specific to Python Interpreter Python Build System with Spaces in file name runs on cmd

```bash
{
    "shell_cmd": "start cmd /C \"(ADD_YOUR_PATH_TO_PYTHON_INTERPRETER_HERE \"$file\" || set /p = Failed execution. Press Enter to exit...) && set /p = Successful execution. Press Enter to exit...\"",
    "file_regex": "^[ ]*File \"(...*?)\", line ([0-9]]*)",
    "selector": "source.python",
    "shell": "true",
}
```

#### 🧿 Generalised Provided By Sublime text Runs Inside Sublime text Itself

```bash
{
    "cmd": ["python", "$file"],
    "selector": "source.python",
    "file_regex": "^\\s*File \"(...*?)\", line ([0-9]*)"
}
```
