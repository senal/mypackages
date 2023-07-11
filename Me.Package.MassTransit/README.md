# Authentication Packages
Common packages relates to MassTransit

## Create and publish package
```powershell
$version="0.0.2"
$owner="senal"
$gh_pat = ["PAT HERE"]

dotnet pack .\Me.Package.MassTransit --configuration Release -p:PackageVersion=$version -p:RepositoryUrl=https://github.com/$owner/mypackages -o .\packages

dotnet nuget push .\packages\Me.Package.MassTransit.$version.nupkg --api-key $gh_pat --source "https://nuget.pkg.github.com/$owner/index.json"
```