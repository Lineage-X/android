Lineage X
===========
[![Download Lineage X](https://a.fsdn.com/con/app/sf-download-button)](https://sourceforge.net/projects/lineage-x/files/latest/download)

Getting started
---------------

To get started with Lineage X, you'll need to get
familiar with [Repo](https://source.android.com/source/using-repo.html) and [Version Control with Git](https://source.android.com/source/version-control.html).

To initialize your local repository use a command like this:
```
repo init -u https://github.com/Lineage-X/android.git -b ten
```
Then to sync up:
```
repo sync -c --force-sync --no-tags --no-clone-bundle -j$(nproc --all) --optimized-fetch --prune
```

Build command
```
. build/envsetup.sh
lunch lineage_$device-userdebug
mka bacon
```

Credits:
[Lineage OS](https://github.com/lineageos)
