# Authentication Packages
Common packages relates to Dapr

## Create and publish package
```powershell
$version="0.0.1"
$owner="senal"
$gh_pat = ["PAT HERE"]

dotnet pack .\Me.Package.Dapr --configuration Release -p:PackageVersion=$version -p:RepositoryUrl=https://github.com/$owner/mypackages -o .\packages

dotnet nuget push .\packages\Me.Package.Dapr.$version.nupkg --api-key $gh_pat --source "https://nuget.pkg.github.com/$owner/index.json"
```