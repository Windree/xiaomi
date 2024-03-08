# Remove bloatware from Redmi Note 10 Pro (sweet) EEA firmware

[Firmware](https://xiaomifirmwareupdater.com/miui/ruby/)

```
adb shell pm disable-user --user 0 com.google.android.gm
adb shell pm disable-user --user 0 com.android.chrome
adb shell pm disable-user --user 0 com.xiaomi.glgm
adb shell pm disable-user --user 0 com.google.android.apps.maps
adb shell pm disable-user --user 0 com.xiaomi.mipicks
adb shell pm disable-user --user 0 com.miui.videoplayer
adb shell pm disable-user --user 0 com.miui.player
adb shell pm disable-user --user 0 com.miui.miservice
adb shell pm disable-user --user 0 com.miui.weather2
adb shell pm disable-user --user 0 com.xiaomi.mipicks
adb shell pm disable-user --user 0 com.mi.globalbrowser
adb shell pm disable-user --user 0 com.google.android.apps.photos
adb shell pm disable-user --user 0 com.google.android.youtube
```
