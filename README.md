# PhotoLabWinUI

vs2019
Winappsdk 1.0+

this code is reference and implement
https://docs.microsoft.com/en-US/windows/apps/windows-app-sdk/migrate-to-windows-app-sdk/case-study-1

for unpackaged setting, 

instead of  

```
StorageFolder appInstalledFolder = Package.Current.InstalledLocation;
StorageFolder picturesFolder = await appInstalledFolder.GetFolderAsync("Assets\\Samples");
```

with 

```
System.IO.Directory.GetCurrentDirectory() + "\\Assets\\Samples";
```
and runtime install
https://docs.microsoft.com/en-US/windows/apps/windows-app-sdk/deploy-unpackaged-apps
