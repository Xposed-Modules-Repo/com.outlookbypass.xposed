# Outlook Device Policy Bypass

[![ko-fi](https://img.shields.io/badge/Support_on-Ko--fi-FF5E5B?logo=ko-fi&logoColor=white)](https://ko-fi.com/takatto)

适用于 Android 的 LSPosed 模块，可绕过 Microsoft Outlook 的 MDM 设备管理/管理员设备要求，无需将手机注册为受管设备即可正常使用 Outlook。已测试支持 Android 15/16 与 Outlook 5.2+。

LSPosed module that kills the MDM device-policy enrollment prompt in **Microsoft Outlook for Android** (`com.microsoft.office.outlook`).

Lets you use Outlook on Android without having to set Outlook as Device Admin.

<img alt="image" src="https://github.com/user-attachments/assets/7367d711-d339-4ac0-bbf9-5a423cf9e668" />


Tested on Android 15 / 16 and Outlook 5.2+.

Built against the modern [libxposed API 101](https://github.com/libxposed/api). Only loads inside the Outlook process (static scope), nothing else gets touched.


## Contributing

Open an issue or PR. Bug reports with the Outlook version + Android version are extra welcome.

Source code: https://github.com/takattowo/OutlookDevicePolicyBypass

## Build (CI)

`.github/workflows/build.yml` builds a signed release APK on every push and PR. Tag a commit `vX.Y.Z` to also publish a GitHub Release.

## Support

If something looks off: `adb logcat -s OutlookPolicyBypass`.

If this saved you from corporate MDM hell, [buy me a coffee](https://ko-fi.com/takatto) ☕
