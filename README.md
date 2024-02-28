# VSCode configuration to run REXX program with Regina REXX Interpreter on Windows system

Click on `Run and Debug` icon in VSCode. Click on `create a launch.json file` and add below configurations.

```
"configurations": [
        {
            "name": "PowerShell Launch Current File",
            "type": "PowerShell",
            "request": "launch",
            "script": "clear; rexx ${file}; echo \"`nProgram ended with exit code $LastExitCode `n\"",
            "cwd": "${cwd}"
        }
    ]
```
To run REXX program opened in the VSCode editor just use shortcut `Ctrl + F5`. Enjoy! 
