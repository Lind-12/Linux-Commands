# Linux-Commands
---
## Aumetar screenlight
aumenta el brillo maximo de la pantalla (eDP Nombre de la pantalla, 1.2 Nivel de brillo)
```
xrandr --output eDP --brightness 1.2
```
nombre de la pantalla, `en este caso es eDP`
```
xrandr
```
```
Screen 0: minimum 320 x 200, current 1920 x 1080, maximum 8192 x 8192
eDP connected primary 1920x1080+0+0 (normal left inverted right x axis y axis) 160mm x 90mm
```
## Ip local y publica
Ip local en este caso es `172.29.76.71`
```
ip a
```
```
wlp3s0:
inet 172.29.76.71/21
```
Ip publica
```
curl ifconfig.me
```
## Dar permiso a un .AppImage/.run
permite ejecupar un `.AppImage/.run` descargado
```
chmod +x ./<Archivo>.AppImage/.run
./<Archivo>.AppImage/.run  (or double click)
```
##
