## TWRP device tree for Lenovo S860 (S860)

Add to `.repo/local_manifests/S860.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
	<project path="device/lenovo/S860" name="android_device_lenovo_S860" remote="liquidporting" revision="android-5.1" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_S860-eng
make -j5 recoveryimage
```