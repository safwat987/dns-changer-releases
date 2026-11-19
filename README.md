# DNS Changer — releases

Download builds of **DNS Changer**, a small Windows 11 app for switching DNS servers, with DNS over HTTPS, a leak check and a health monitor.

## Download

Get the latest version from [Releases](../../releases/latest):

| File | Use it if |
|---|---|
| `DnsChanger.exe` | You have the [.NET 8 Desktop Runtime](https://dotnet.microsoft.com/download/dotnet/8.0) (small download) |
| `DnsChanger-portable.exe` | You want one file that runs on any Windows 10/11 x64 PC |

The app asks for administrator rights because changing DNS settings needs them.

## Verify a download

Each release has a `SHA256SUMS.txt`. In PowerShell:

```powershell
Get-FileHash .\DnsChanger.exe -Algorithm SHA256
```

The hash should match the line for that file. The app's built-in updater does this check automatically before installing an update.

The files aren't code-signed, so Windows SmartScreen may show a warning the first time; choose "More info" → "Run anyway".
