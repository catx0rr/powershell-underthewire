# Underthewire.tech

Century 1

- The format is as follows: **.*.*****.****
- Include all periods
- Be sure to look for build version and NOT Powershell version

```
$PSVersionTable.BuildVersion | ForEach-Object {"$_"}

$PSVersionTable.BuildVersion | % {"$_"}

```

Century 2

- If the name of the cmdlet is "get-web" and the file on the desktop is named "1234" the password would be "get-web1234"

```
Get-ChildItem | ForEach-Object {$_.Name}

Get-ChildItem | ForEach-Object {"$_"}

(Get-ChildItem).Name | Select-String -Pattern "^[0-9]{0,}$"

password: invoke-webrequest443
```

Century 3

- The password for Century4 is the number of files on the desktop

```
Get-ChildItem | Measure-Object -Line | ForEach-Object {$_.Lines}


```

Century 4

- The password for Century5 is the name of the file within a directory on the desktop that has spaces in its name.
- The password will be lowercase no matter how it appears on the screen.

```
Get-ChildItem -Filter "Can You Open Me" -Recurse | Get-ChildItem | Foreach-Object {$_.Name}
```


