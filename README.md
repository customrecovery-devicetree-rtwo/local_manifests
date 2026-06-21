# Local manifests for Motorola rtwo

Use this with an OrangeFox/TWRP Android 12.1 source tree.

```bash
mkdir -p .repo/local_manifests
cp rtwo.xml .repo/local_manifests/rtwo.xml
repo sync -c --force-sync --no-clone-bundle --no-tags
source build/envsetup.sh
lunch orangefox_rtwo-eng
mka recoveryimage
```
