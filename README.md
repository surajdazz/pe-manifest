# Pixel Experience #

### Sync ###

```bash

# Initialize local repository
repo init --depth=1 --no-repo-verify -u https://github.com/surajdazz/pe-manifest.git --git-lfs -b thirteen-plus

# Sync
repo sync -c --no-clone-bundle --optimized-fetch --prune --force-sync -j$(nproc --all)
```

### Build ###

```bash

# Set up environment
$ . build/envsetup.sh

# Choose a target
$ lunch aosp_$device-userdebug

# Build the code
$ mka bacon -jX
```

### Submitting Patches ###

Patches are always welcome! Please submit your patches to our Gerrit.

[Gerrit push guide](https://wiki.pixelexperience.org/help/submit-patch/)