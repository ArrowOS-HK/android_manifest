<img src="https://github.com/ArrowOS/getting_started/blob/master/misc/logo.png?raw=true">

# ArrowOS (EXPERIMENTAL BRANCH)

 Getting Started
---------------
**NOTE: THIS BRANCH IS EXPERIMENTAL, use arrow-13.1 branch for buildable source.**
To get started with the ArrowOS sources, you'll need to get
familiar with [Git and Repo](https://source.android.com/setup/build/downloading).

To initialize your local repository, use command:

```bash
repo init -u https://github.com/ArrowOS-HK/android_manifest.git -b arrow-13.1_ext
```

Then sync up:

```bash
repo sync
```

Add-Ons
-------------------
Before building the system, add this prop to your device system.prop.

```bash
# Hardware Description
ro.ext.maintainer=(your name)
ro.device.maintainer_link=(telegram profile link)
ro.ext.model=(example M1908C3JH)      
ro.ext.processor=(example Snapdragon 665)   
ro.ext.battery=(example 4000)
ro.ext.camera.front=(example 13)
ro.ext.camera.rear=(example 48,8,2,2)
```

Building the System
-------------------
 Initialize the ROM environment with the envsetup.sh script.

```bash
. build/envsetup.sh
```

Lunch your device after cloning all device sources if needed.

```bash
lunch arrow_devicecodename-buildtype
```

Start compilation

```bash
mka otapackage
```

OR

```bash
mka bacon
```

**You can also refer to our detailed guides as listed below:**

[How to compile ArrowOS from source](https://blog.arrowos.net/android/arrowos/guides/compilation-guide)

[How to submit patches to ArrowOS Gerrit](https://blog.arrowos.net/android/arrowos/guides/how-to-submit-patches-to-arrowos-gerrit)

[Apply for Maintainership](https://blog.arrowos.net/android/arrowos/community/apply-for-maintainership) OR [Submit device for community builds](https://blog.arrowos.net/android/arrowos/news/introducing-community-builds)

To check thread template refer [**HERE**](https://raw.githubusercontent.com/ArrowOS/documentation/master/thread_template.txt)

---------------------------------------------------------------------------------------------------------------------

[ArrowOS Website](https://www.arrowos.net) | [ArrowOS Blog](https://blog.arrowos.net)

---------------------------------------------------------------------------------------------------------------------
