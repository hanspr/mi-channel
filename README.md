# Channel repo for mi-ide

This repo is for developers of plugins for mi-ide

If you do not know about mi-ide, visit : https://github.com/hanspr/mi-ide

* Clone this repo
* Add your repo in plugins.json

Add a line like this:

```json
[
  "https://raw.githubusercontent.com/hanspr/mi-sources/master/plugins/repo.json",
  "https://raw.githubusercontent.com/miaccount/mirepo/master/...../repo.json"
]
```

Submit a merge to add your repo

At your repository, create a repo.json similar to : https://github.com/hanspr/mi-sources/blob/master/plugins/repo.json

To publish your plugins

```json
[{
  "Name": "plugin name",
  "Author": "your github account",
  "Filetype": "file type",
  "Description": "Your breif description",
  "Tags": ["language"],
  "Versions": [
    {
      "Version": "1.0.0",
      "Url": "https://raw.githubusercontent.com/your account/your repo/master/file.zip",
      "Require": {
        "micro": ">=1.1.0"
      }
    }
  ]
}]
```

## Zip file

Your file should be a zip of your plugin directory without absolute paths, example:

````
General description

directory
    plugin.lua
    settings.json


Example

javascript
	javascript.lua
	settings.json

````
