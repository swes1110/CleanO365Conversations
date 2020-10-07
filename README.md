# CleanO365Conversations

CleanUnifiedGroup is a simple python script to delete all of the conversations from a given Unified Group (O365 Group).

## Dependencies

Python 3.x

##### The following modules are required

* MSAL `v1.5.0`
```
pip install msal
```

*Listed versions are validated with this application, other's may work but have not been tested*

## Configuration

### Azure AD Configuration

To utilize this application you must configure an enterprise application registration with the following settings:
1. Application must be configured with redirect URI's set to "Mobile and desktop applications" and not the default of "web" for public client authentication ![AzurePortalScreenshot](https://i.imgur.com/dXFb08o.png)
1. Application must be set to "treat application as a public client![AzurePortalScreenshot](https://i.imgur.com/ToN6RIT.png)

### Configuration File

Rename the configuration file from ParametersSample.json to Parameters.json and fill in the following values
```
"client_id": "{YOUR_CLIENT_ID}",
"group_id": "{YOUR_GROUP_ID}"
```


## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
GNU General Public License v3.0
