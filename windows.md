# Windows Commands
-----------------------------

This is a useful file where you can find useful commands to use on Powershell and cmd on windows machines

- **Delete a folder with files inside it**:

```{pwershell}
Remove-Item -Recurse -Force SilentlyContinue <<Folder path>>

Remove-Item -Recurse -Force -ErrorAction SilentlyContinue <<Folder path>> 
```
