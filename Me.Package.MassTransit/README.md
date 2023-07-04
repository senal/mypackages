# Authentication Packages
Common packages relates to MassTransit

## Create and publish package
```powershell
$version="0.0.1"
$owner="senal"
dotnet pack .\Me.Package.MassTransit --configuration Release -p:PackageVersion=$version -p:RepositoryUrl=https://github.com/$owner/mypackages -o .\packages
```