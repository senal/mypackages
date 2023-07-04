# Authentication Packages
Common packages relates to Database

## Create and publish package
```powershell
$version="0.0.1"
$owner="senal"
dotnet pack .\Me.Package.Dapr --configuration Release -p:PackageVersion=$version -p:RepositoryUrl=https://github.com/$owner/mypackages -o .\packages
```