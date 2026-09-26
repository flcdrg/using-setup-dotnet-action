# using-setup-dotnet-action

Examples using the [action/setup-dotnet](https://github.com/marketplace/actions/setup-net-core-sdk) GitHub Action

## Setup

To download and install packages from a repository, your personal access token (classic) must have the `read:packages` scope.

[NuGet.Config locations](https://learn.microsoft.com/en-us/nuget/consume-packages/configuring-nuget-behavior)

### Windows

```powershell
dotnet nuget add source --username USERNAME --password YOUR-PAT --store-password-in-clear-text --name github "https://nuget.pkg.github.com/flcdrg/index.json" --configfile $env:appdata\NuGet\NuGet.Config
```

### macOS

```bash
dotnet nuget add source --username USERNAME --password YOUR-PAT --store-password-in-clear-text --name github "https://nuget.pkg.github.com/flcdrg/index.json" --configfile  ~/.nuget/NuGet/NuGet.Config
```
