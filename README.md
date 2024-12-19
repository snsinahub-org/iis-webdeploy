# iis-webdeploy

This action helps to deploy entire application to a local or remote IIS server. Moreover, this action supports to add or remove a file to/from IIS server as well, this feature is specifically useful when you try to make a website offline or bring it back to online.

```YAML
  - name: publish to server
    uses: snsinahub-org/iis-webdeploy@v1.0.0
    with:
      source: <source-file>
      destination: <destination-folder>
      remote_url: <remote-iis-server>
      username: <remote-server-username>
      password: <remote-server-password>
      type: <type-of-deployment>
```

## Supported type of seployments 

- add_appoffline: upload a file to remote server
- del_appoffline: delete a file from server
- full: deploy entire application (.zip format) to server

## External link 

https://learn.microsoft.com/en-us/powershell/scripting/windows-powershell/wmf/setup/install-configure?view=powershell-7.3
