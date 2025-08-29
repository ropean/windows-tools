### Ropean Windows Tools

A curated list and binary home for Ropean's small Windows utilities. If you prefer package management, you can install all apps via the dedicated Scoop bucket: `https://github.com/ropean/scoop-ropean`.

### Quick start

- **Direct download**: Grab `.exe` files from this repository or from Releases.
- **Install with Scoop** (recommended):

```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
irm get.scoop.sh | iex

scoop bucket add ropean https://github.com/ropean/scoop-ropean

# Install any app
scoop install bestpwd
scoop install cssimagedownload
scoop install filesplit
scoop install httpstatus
scoop install music2sd
scoop install myexplorer
scoop install myhosts
scoop install suckcolor

# Upgrade Scoop and apps
scoop update
scoop update <app>
```

### Available apps

- **bestpwd**: Password management utility (`scoop install bestpwd`)
- **cssimagedownload**: Download images referenced in CSS (`scoop install cssimagedownload`)
- **filesplit**: Split large files into smaller chunks (`scoop install filesplit`)
- **httpstatus**: Check HTTP status codes (`scoop install httpstatus`)
- **music2sd**: Copy music to SD/removable devices (`scoop install music2sd`)
- **myexplorer**: Enhanced file explorer (`scoop install myexplorer`)
- **myhosts**: Hosts file editor (`scoop install myhosts`)
- **suckcolor**: Color picker utility (`scoop install suckcolor`)

### Versioning & updates

- Apps are versioned with tags like `vX.Y.Z`.
- Scoop manifests in the bucket are configured with GitHub `checkver` and `autoupdate` to pick up new releases automatically.

### Verify downloads

```powershell
Get-FileHash .\YourDownloadedFile.exe -Algorithm SHA256
```

### Contributing

- **Packaging changes** (hashes, versions, new apps): open a PR in the Scoop bucket (`bucket/` manifests) at `https://github.com/ropean/scoop-ropean`.
- **Bugs or feature requests** for the apps: open an issue in this repository.

### License

Proprietary. See `LICENSE.txt`.
