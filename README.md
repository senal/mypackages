# Adding nuget (github) package source to a project

Note: USERNAME parameter is not important here, just add it for the sake of ading it

```powershell
$owner="senal"
$gh_pat="[PAT HERE]"

dotnet nuget add source --username USERNAME --password $gh_pat --store-password-in-clear-text --name github "https://nuget.pkg.github.com/$owner/index.json"
```
