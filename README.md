# BepInEx for Stoker

[BepInEx](https://github.com/BepInEx/BepInEx) 5, the plugin and mod loader for Unity games, as `app.stokerhq.bepinex` in
the StokerHQ plugin registry ([StokerHQ/plugins](https://github.com/StokerHQ/plugins)). A [Stoker](https://github.com/StokerHQ)
instance installs it from there and lays it into a game beside the mods that need it.

**Nothing here is changed or rebuilt.** Each release of this repository carries BepInEx's own release zips for that
version, exactly as BepInEx published them: `package.yaml` names each file and pins its SHA-256, and CI fetches them
from BepInEx's release, checks them, and attaches them to the release here. The registry entry names BepInEx's
repository and the commit of its tag as the source.

BepInEx is by the BepInEx team. For BepInEx itself - its documentation, issues and releases - see
[BepInEx/BepInEx](https://github.com/BepInEx/BepInEx).

## Platforms

| File | |
|---|---|
| `BepInEx_win_x64_<version>.zip` | Windows, 64-bit games |
| `BepInEx_win_x86_<version>.zip` | Windows, 32-bit games |
| `BepInEx_linux_x64_<version>.zip` | Linux, 64-bit games |

## A new BepInEx version

1. Change `package.yaml`: the version, the upstream tag and its commit, and each file with the SHA-256 BepInEx's release
   lists for it.
2. Merge, then publish a release here tagged `v<version>`. CI checks every file and attaches it.

## Licence

BepInEx is licensed under the GNU Lesser General Public License 2.1 (`LICENSE`, BepInEx's own). Its source is at
[BepInEx/BepInEx](https://github.com/BepInEx/BepInEx), at the commit `package.yaml` names.