Master Manifests
========================

Getting Started
---------------

To get started with Android/Master, you'll need to get familiar with [Source Control Tools](https://source.android.com/setup/develop).

To initialize your local repository using the AtigaOS trees, use a command like this:
```bash
repo init --depth=1 -u https://github.com/aepranata/sample_manifest.git -b master --git-lfs
```

Clone this repository in `.repo/local_manifests`:
```bash
git clone --single-branch -b master https://github.com/aepranata/atiga_manifests.git .repo/local_manifests
```

Then to sync up:
```bash
repo sync -c --no-clone-bundle --no-tags --optimized-fetch --prune --force-sync -j8
```
