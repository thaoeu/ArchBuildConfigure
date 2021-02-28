## 键盘布局

### Xorg

#### 临时
```
setxkbmap dvorak &
```

#### 长期


### SDDM

#### 长期
编辑文件：`/etc/X11/xorg.conf.d/00-keyboard.conf`

```
Section "InputClass"
        Identifier "system-keyboard"
        MatchIsKeyboard "on"
        Option "XkbLayout" "us"
        Option "XkbModel" "pc104"
        Option "XkbVariant" "dvorak"
        Option "XkbOptions" "grp:alt_shift_toggle"
EndSection
```

### TTY

#### 临时
```
loadkeys dvorak
```

编辑文件：`/etc/vconsole.conf`
```
KEYMAP=dvorak
```

