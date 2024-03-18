# Remove bloatware from Redmi Note 12 Pro Plus (rubypro) Global firmware

[Firmware](https://xiaomifirmwareupdater.com/miui/ruby/)

patse and run fillowing code in powershell

```pwsh
`
"com.android.chrome",
"com.facebook.appmanager",
"com.facebook.services",
"com.facebook.system",
"com.google.android.adservices.api",
"com.google.android.apps.maps",
"com.google.android.apps.photos",
"com.google.android.apps.safetyhub",
"com.google.android.apps.subscriptions.red",
"com.google.android.gm",
"com.google.android.youtube",
"com.mi.globalbrowser",
"com.mi.globalminusscreen",
"com.miui.miservice",
"com.miui.msa.global",
"com.miui.player",
"com.miui.videoplayer",
"com.miui.weather2",
"com.xiaomi.discover",
"com.xiaomi.glgm",
"com.xiaomi.mipicks" | %{
	Write-Host "Package:" $_
	Write-Host "Uninstall package..."
	&adb shell pm uninstall --user 0 $_
	Write-Host
}
```

Remove additional packages

```pwsh
`
"com.miui.cleaner",
"com.miui.calculator",
"com.xiaomi.payment",
"com.miui.notes",
"com.miui.cloudservice",
"com.miui.yellowpage",
"com.xiaomi.joyose",
"com.tencent.soter.soterserver",
"com.miui.cloudbackup" | %{
	Write-Host "Package:" $_
	Write-Host "Uninstall package..."
	&adb shell pm uninstall --user 0 $_
	Write-Host
}
```

Remove SMS/MMS messanger to replace with FOSS [SMS Messanger](https://f-droid.org/en/packages/com.simplemobiletools.smsmessenger/)

```pwsh
`
"com.android.mms",
"com.google.android.apps.messaging" | %{
	Write-Host "Package:" $_
	Write-Host "Uninstall package..."
	&adb shell pm uninstall --user 0 $_
	Write-Host
}
```

Remove Dialer/Phone to replace with FOSS [Dialler](https://f-droid.org/en/packages/com.simplemobiletools.dialer/)

```pwsh
`
"com.google.android.dialer" | %{
	Write-Host "Package:" $_
	Write-Host "Uninstall package..."
	&adb shell pm uninstall --user 0 $_
	Write-Host
}
```
