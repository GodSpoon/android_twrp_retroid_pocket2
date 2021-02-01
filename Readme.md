Twrp device tree for the Retroid Pocket 2

Install repo
https://android.googlesource.com/tools/repo

## Getting Started ##
---------------

To get started with OMNI sources to build TWRP, you'll need to get
familiar with [Git and Repo](https://source.android.com/source/using-repo.html).

To initialize your local repository using the OMNIROM trees to build TWRP, use a command like this:

    repo init -u git://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git -b twrp-8.1
    
To initialize a shallow clone, which will save even more space, use a command like this:

    repo init --depth=1 -u git://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git -b twrp-8.1

Then to sync up:

    repo sync

Then to build:

     cd <source-dir>; export ALLOW_MISSING_DEPENDENCIES=true; . build/envsetup.sh; lunch omni_<device>-eng; mka recoveryimage

Reference for build/repo 
https://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni/tree/twrp-8.1


Based on https://github.com/mt8163/android_device_bq_aquaris_m8 and https://github.com/Black-Seraph/android_twrp_gpd_gpd_en


Thanks to @R0rt1z2 & @488315 for helping on this!
Special thanks to Retroid for releasing kernel source code!
Thanks to @thoramund(github.com/thoramund) for tweaking the 320x240 theme to work with Retroid Pocket 2
