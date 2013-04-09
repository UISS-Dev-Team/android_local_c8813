Local manifests for building CyanogenMod 10.1 for Huawei Device

How to build:
-------------

Initialize repo:

    repo init -u ssh://<username>@review.mfunz.com:29418/MoKee/android.git -b jb-mr1_mkt  <username>注册的名称
    curl -L -o .repo/local_manifests/local_manifest.xml -O -L https://raw.github.com/UISS-Dev-Team/android_local_manifest/mk-4.22/local_manifest.xml
    repo sync

Compile:

    . build/envsetup.sh && brunch device_name


如何打包：
-------------

初始化代码:

    repo init -u ssh://<username>@review.mfunz.com:29418/MoKee/android.git -b jb-mr1_mkt  <username>注册的名称
    curl -L -o .repo/local_manifests/local_manifest.xml -O -L https://raw.github.com/UISS-Dev-Team/android_local_manifest/mk-4.22/local_manifest.xml
    repo sync

编译：

    . build/envsetup.sh && brunch 机器代号（如c8813）

