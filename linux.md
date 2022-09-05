# WSL only

Open anything from wsl terminal as if it was double clicked in windows, even opening current dir in explorer (i.e. `start .`)

```
alias start="powershell.exe /c start"
```

# Any environment

## Batch processing of files

Example: pretty-print all XML files in a folder and place beautified versions in a /formatted folder while keeping the original names

```
mkdir formatted; ls -1 *fr.xml | xargs -l bash -c 'xmllint --format $0 > formatted/$0.xml'
```

