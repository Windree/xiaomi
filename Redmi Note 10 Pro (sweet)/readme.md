# Remove bloatware from Redmi Note 10 Pro (sweet) EEA firmware

[Firmware](https://xiaomifirmwareupdater.com/miui/sweet/stable/V14.0.9.0.TKFEUXM/)

Run following in powershell

```pwsh
`
"com.android.chrome",
"com.facebook.appmanager",
"com.facebook.services",
"com.facebook.system",
"com.google.android.adservices.api",
"com.google.android.apps.googleassistant",
"com.google.android.apps.maps",
"com.google.android.apps.safetyhub",
"com.google.android.apps.subscriptions.red",
"com.google.android.apps.turbo",
"com.google.android.apps.wellbeing",
"com.google.android.gm",
"com.google.android.projection.gearhead",
"com.google.android.youtube",
"com.google.mainline.adservices",
"com.google.mainline.telemetry",
"com.mi.globalminusscreen",
"com.miui.bugreport",
"com.miui.calculator",
"com.miui.cleaner",
"com.miui.cloudbackup",
"com.miui.cloudservice",
"com.miui.compass",
"com.miui.face",
"com.miui.gallery",
"com.miui.micloudsync",
"com.miui.miservice",
"com.miui.misound",
"com.miui.msa.global",
"com.miui.notes",
"com.miui.phrase",
"com.miui.player",
"com.miui.qr",
"com.miui.systemui.carriers.overlay",
"com.miui.touchassistant",
"com.miui.videoplayer",
"com.miui.weather2",
"com.miui.yellowpage",
"com.xiaomi.cameratools",
"com.xiaomi.glgm",
"com.xiaomi.joyose",
"com.xiaomi.mipicks" | %{
	Write-Host "Package:" $_
	Write-Host "Uninstall package..."
	&adb shell pm uninstall --user 0 $_
	Write-Host
}
```
