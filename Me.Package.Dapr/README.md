# Authentication Packages
Common packages relates to authentication

## Create and publish package
```powershell
$version="0.0.1"
$owner="senal"
dotnet pack .\My.Package.Dapr --configuration Release -p:PackageVersion=$version -p:RepositoryUrl=https://github.com/$owner/mypackages -o .\packages
```