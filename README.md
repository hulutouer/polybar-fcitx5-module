### This module is used to display the status of fcitx5 input method (zh or en)


#### preview
![[https://github.com/hulutouer/polybar-fcitx5-module/blob/main/screenshot/fcitx5.gif]]

#### and
![[https://github.com/hulutouer/polybar-fcitx5-module/blob/main/screenshot/fcitx5-2.gif]]



### Usage

#### Copy to the configuration file `config. ini`, and call
```
[module/fcitx5]
type = custom/script
format-prefix = " "
exec = [[ $(fcitx5-remote) -eq 2 ]] &&echo "zh" || echo "en"
interval = 0.3
format-prefix-foreground = ${colors.primary}
```

#### master file import ..., and call
```
include-file = PATH/fcitx5.ini
```
