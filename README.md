# p930-twrp-omni
LG Nitro HD/Optimus LTE/True HD LTE family twrp device tree

# How to build
```
repo init --depth=1 -u git://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git -b twrp-6.0

mkdir -p .repo/local_manifests

wget -O .repo/local_manifests/local_manifests.xml http://raw.githubusercontent.com/bjsiu/p930-twrp-omni/master/local_manifests.xml

repo sync -j4

source build/envsetup.sh

lunch omni_p930-eng

make -j4 clobber && make -j4 recoveryimage
```

# License
Apache License v2.0 (for all files)
