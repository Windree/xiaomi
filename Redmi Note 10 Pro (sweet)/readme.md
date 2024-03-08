# Remove bloatware from Redmi Note 10 Pro (sweet) EEA firmware

## [Firmware](https://xiaomifirmwareupdater.com/miui/sweet/stable/V14.0.9.0.TKFEUXM/)

adb shell pm disable-user --user 0 com.google.android.gm
adb shell pm disable-user --user 0 com.google.android.apps.subscriptions.red
adb shell pm disable-user --user 0 com.google.android.apps.googleassistant
adb shell pm disable-user --user 0 com.android.chrome
adb shell pm disable-user --user 0 com.xiaomi.glgm
adb shell pm disable-user --user 0 com.google.android.apps.maps
adb shell pm disable-user --user 0 com.xiaomi.mipicks
adb shell pm disable-user --user 0 com.miui.videoplayer
adb shell pm disable-user --user 0 com.miui.player
adb shell pm disable-user --user 0 com.google.android.apps.safetyhub
adb shell pm disable-user --user 0 com.miui.service
adb shell pm disable-user --user 0 com.miui.miservice
adb shell pm disable-user --user 0 com.miui.weather2
adb shell pm disable-user --user 0 com.google.android.youtube
