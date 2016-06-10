## TWRP device tree for Xiaomi Redmi Note 3 (MTK variant)

Add to `.repo/local_manifests/hennessy.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
	<project path="device/xiaomi/hennessy" name="android_device_xiaomi_hennessy" remote="TeamWin" revision="android-5.1" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_hennessy-eng
make -j5 recoveryimage
```
