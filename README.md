#### __Download source:__

```
$ mkdir huawei_AGS-W09
$ cd huawei_AGS-W09
$ repo init -u https://github.com/secuflag/manifest_huawei_AGS-W09.git
$ repo sync -j12
```

#### __Compile Kernel:__

```
$ cd kernel
$ export ARCH=arm64
$ export CROSS_COMPILE=aarch64-linux-android-
$ export PATH=$PATH:/path/to/aarch64-linux-android-4.9/bin
$ make merge_msm8937_64_defconfig
$ make Image.gz-dtb
```
