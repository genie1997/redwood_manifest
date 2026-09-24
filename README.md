# Local manifest for redwood

POCO X5 Pro 5G, Android 17.

Initialize the ROM tree first, then clone this into it and sync:

```bash
git clone https://github.com/genie1997/redwood_manifest -b seventeen .repo/local_manifests
repo sync -c --no-clone-bundle --no-tags --optimized-fetch --prune --force-sync -j$(nproc --all)
```
