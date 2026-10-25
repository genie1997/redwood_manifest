# Local manifest for redwood

POCO X5 Pro 5G, Android 17.

Initialize the ROM tree first, then clone this into it and sync:

```bash
git clone https://github.com/genie1997/redwood_manifest -b seventeen .repo/local_manifests
repo sync -c --no-clone-bundle --no-tags --optimized-fetch --prune --force-sync -j$(nproc --all)
```

Every tree is pinned to a commit. The trees are shallow (`clone-depth="1"`), so a pin that is no
longer a branch tip falls back to a full clone.
