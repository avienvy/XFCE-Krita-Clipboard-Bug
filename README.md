# XFCE-Krita-Clipboard-Bug
Simple fix that cause krita crash while paste (ctrl+v) on XFCE desktop environment

You can create desktop entry manually or download from the repository directly, then simply add it to your session startup to make it persist on login.

```
[Desktop Entry]
Version=1.0
Type=Application
Name=clipboard bug
Comment=
Exec=env XFSETTINGSD_NO_CLIPBOARD=1 xfsettingsd --replace
Icon=
Path=
Terminal=false
StartupNotify=false
```

Please refer to this link for further update https://gitlab.xfce.org/xfce/libxfce4ui/-/issues/141
