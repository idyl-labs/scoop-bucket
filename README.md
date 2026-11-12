# Idyl Labs Scoop bucket

Scoop manifests for Idyl Labs command-line tools on Windows, for amd64 and
arm64. Scoop picks the build for the machine it runs on.

| Manifest | Installs |
| --- | --- |
| `idyl` | `idyl`, the command-line client for IDYL |
| `purlview` | `purlview`, which shares a running app for live feedback |

Add the bucket once:

```powershell
scoop bucket add idyl-labs https://github.com/idyl-labs/scoop-bucket
```

## idyl

```powershell
scoop install idyl
scoop update idyl
scoop uninstall idyl
```

The manifest downloads each release from IDYL's download site,
`get.idyl.sh`.

## purlview

```powershell
scoop install purlview
scoop update purlview
scoop uninstall purlview
```

Updating Purlview stops its local daemon and ends any active shares; start
a share again afterwards.

## How the manifests are published

Each project's release workflow writes its manifest for every stable release
and commits it here, so a change made directly to a manifest is replaced by
the next release. Prereleases are not published to the bucket.
