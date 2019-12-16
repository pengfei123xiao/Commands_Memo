#### `tasks.json` for vscode
```
{
    "version": "2.0.0",
    "tasks": [
        {
            "label": "list environment",
            "type": "shell",
            "command": "pip freeze; python --version; which python",
            "args": [],
            "group": "build",
            "problemMatcher": []
        },
        {
            "label": "update python environment",
            "type": "shell",
            "command": "conda env update -f environment.yml",
            "args": [],
            "group": "build",
            "problemMatcher": []
        },
        {
            "label": "build python environment",
            "type": "shell",
            "command": "conda env create -f environment.yml",
            "args": [],
            "group": "build",
            "problemMatcher": []
        },
        {
            "label": "activate python environment",
            "type": "shell",
            "command": "conda activate ch_import",
            "args": [],
            "group": "build",
            "problemMatcher": []
        },
        {
            "label": "run data import",
            "type": "shell",
            "command": "python import_to_clickhouse.py",
            "args": [],
            "group": "build",
            "problemMatcher": []
        }
    ]
 }
 ```
