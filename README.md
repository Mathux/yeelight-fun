# yeelight-fun
Some fun script to interface my yeelight RGB bulb. 


## How to use
### To change the brightness into x%

```bash
yeelight set x
```
### Toggle on/off
```bash
yeelight toggle 0
```

## i3wm mode
Changing brightness with keybord.

Put in i3 config

```
mode "yeelight" {
     bindsym at exec --no-startup-id /home/mathis/apps/yeelight set 0
     bindsym 1 exec --no-startup-id /home/mathis/apps/yeelight set 10
     bindsym 2 exec --no-startup-id /home/mathis/apps/yeelight set 20
     bindsym 3 exec --no-startup-id /home/mathis/apps/yeelight set 30
     bindsym 4 exec --no-startup-id /home/mathis/apps/yeelight set 40
     bindsym 5 exec --no-startup-id /home/mathis/apps/yeelight set 50
     bindsym 6 exec --no-startup-id /home/mathis/apps/yeelight set 60
     bindsym 7 exec --no-startup-id /home/mathis/apps/yeelight set 70
     bindsym 8 exec --no-startup-id /home/mathis/apps/yeelight set 80
     bindsym 9 exec --no-startup-id /home/mathis/apps/yeelight set 90
     bindsym 0 exec --no-startup-id /home/mathis/apps/yeelight set 100

     bindsym t exec --no-startup-id /home/mathis/apps/yeelight toggle 0

     bindsym Escape mode "default"
}

bindsym --release F7 mode "yeelight"
```