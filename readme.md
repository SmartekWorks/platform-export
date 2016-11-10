### Build

`make.sh`

### Usage

`java -jar PlatformExport.jar <path to config file> <path to target folder>`

### Config file

#### Config parameters

* `serverUrl`: the URL of SWATHub Server URL, such as http://www.swathub.com/
* `username`: the username of SWATHub Server
* `apiKey`: the api key for the user, same as the key for execution node
* `workspaceOwner`: the owner's username of the target workspace to export
* `workspaceName`: the name of the target workspace
* `setID`: the unique ID of the test set in the target workspace, which can be got from the test set url. For instance, the set ID is **9** in the url `http://swathub.com/app/support/samples/scenarios/set/9`
* `tags`: tags filtering the scenarios to export, separated by comma.
* `status`: the list of result status, `finished`, `failed`, `ok` or `ng`
* `platforms`: the list of the platforms to export
* `maxSize`: the max size of platforms to show in one line

#### Sample config file

```
{
  "serverUrl": "http://swathub.com/",
  "username": "tester",
  "apiKey": "A7185B82DB6A4EFC9006",
  "workspaceOwner": "support",
  "workspaceName": "samples",
  "setID": "9",
  "tags": "demo, sample",
  "status": [
    "ok",
    "finished"
  ],
  "platforms": [
    "Windows 10 + Firefox",
    "Windows 10 + Internet Explorer 11",
    "Windows 10 + Chrome"
  ]
}
```

### Available platforms

* Windows + Internet Explorer 6
* Windows + Internet Explorer 7
* Windows + Internet Explorer 8
* Windows + Internet Explorer 9
* Windows + Internet Explorer 10
* Windows + Internet Explorer 11
* Windows + Firefox
* Windows + Chrome
* Windows XP + Internet Explorer 6
* Windows XP + Internet Explorer 7
* Windows XP + Internet Explorer 8
* Windows XP + Firefox
* Windows XP + Chrome
* Windows 7 + Internet Explorer 8
* Windows 7 + Internet Explorer 9
* Windows 7 + Internet Explorer 10
* Windows 7 + Internet Explorer 11
* Windows 7 + Firefox
* Windows 7 + Chrome
* Windows 8 + Internet Explorer 10
* Windows 8 + Internet Explorer 11
* Windows 8 + Firefox
* Windows 8 + Chrome
* Windows 8.1 + Internet Explorer 11
* Windows 8.1 + Firefox
* Windows 8.1 + Chrome
* Windows 10 + Internet Explorer 11
* Windows 10 + Firefox
* Windows 10 + Chrome
* Mac OSX + Safari
* Mac OSX + Firefox
* Mac OSX + Chrome
* Linux + Firefox
* Linux + Chrome
