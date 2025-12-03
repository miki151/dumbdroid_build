
## Building TrebleDroid-based LineageOS GSIs ##

Set up your environment by referring to [LineageOS Wiki](https://wiki.lineageos.org/devices/TP1803/build) (mainly "Install the build packages" and "Install the repo command").

Create a new working directory for your LineageOS build and navigate to it:

    mkdir dumbdroid_build; cd dumbdroid_build

Initialize your LineageOS workspace:

    repo init -u https://github.com/LineageOS/android.git -b lineage-21.0 --git-lfs

Clone both this and the patches repos:

    git clone https://github.com/miki151/dumbdroid_build lineage_build_unified
    git clone https://github.com/miki151/dumbdroid_patches lineage_patches_unified

Finally, start the build script - for example, to build all supported Dumbdroid variants:

    bash lineage_build_unified/buildbot_unified.sh treble DG31 DG30 DV31 DV30

Be sure to update the cloned repos from time to time!

---
