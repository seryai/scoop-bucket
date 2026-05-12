# scoop-bucket

Scoop bucket for [Sery Link](https://sery.ai).

## Install

```powershell
scoop bucket add seryai https://github.com/seryai/scoop-bucket
scoop install sery-link
```

## Update the manifest for a new release

1. Download the MSI from the GitHub release.
2. Compute SHA256:
   ```powershell
   Get-FileHash Sery.Link_<version>_x64_en-US.msi -Algorithm SHA256
   ```
3. Edit `bucket/sery-link.json` — bump `version` and `hash`.
4. Commit and push.
