# iis-webdeploy

This GitHub Action helps deploy an entire application to a local or remote IIS server. Additionally, it supports adding or removing files from the IIS server, which is particularly useful for taking a website offline or bringing it back online.

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

## Supported type of deployments 

- add_appoffline: upload a file to remote server
- del_appoffline: delete a file from server
- full: deploy entire application (.zip format) to server

## External link 

For more information, visit  [Microsoft documentation](https://learn.microsoft.com/en-us/powershell/scripting/windows-powershell/wmf/setup/install-configure?view=powershell-7.3)
