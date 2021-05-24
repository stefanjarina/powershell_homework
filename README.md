# PowerShell Homework

## Exercise

1. Install IIS application
    - you can find a .net "hello world" application in zip
      - application is zipped together with folder we do not want to deploy
        - extract everything from zip except folder `NOT4DEPLOYMENT`
    - application must be in it's own pool
    - application must be under "Default Website"
2. Change `Web.config`
    - add the lines to configuration section according to next example
3. We will run the script on clean Windows Server with 5.1 powershell (we can also use Powershell 7+ if needed)

```xml
<?xml version="1.0" encoding="utf-8"?>
<configuration>
  ...
  <appSettings>
    <add name="UserName" value="ImbaUser" />
    <add name="PasswordHash" value="xxx" />
  </appSettings>
</configuration>
```  

## Variations

- if you do not have a server at your disposal for testing during script development:
  - it can run on your PC, laptop, whatever
  - you can also use virtual machine

## In case of issues

- in case application for some reason does not work, you don't need to fix it, for us only script/code is important, so only script must work
- in case of any questions feel free to contact me via email, or call
