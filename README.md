## TWRP device tree for Galaxy S7 edge (SC-02H)

Add to `.repo/local_manifests/hero2qltedcm.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
	<project path="device/samsung/hero2qltedcm" name="android_device_samsung_hero2qltedcm" remote="TeamWin" revision="android-6.0" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_hero2qltedcm-eng
make -j5 recoveryimage
```

Kernel sources are available at: https://github.com/jcadduono/android_kernel_samsung_msm8996/tree/twrp-6.0
