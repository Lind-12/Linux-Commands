# Linux-Commands
---
## Aumentar screenlight
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
## instalar oh-my-posh
instala oh-my-posh
```
curl -s https://ohmyposh.dev/install.sh | sudo bash -s
```
instalar font
```
oh-my-posh font install
```
instalar thema pasos
1. descargar los temas
```
mkdir ~/.poshthemes
wget https://github.com/JanDeDobbeleer/oh-my-posh/releases/download/v18.15.0/themes.zip -O ~/.poshthemes/themes.zip
unzip ~/.poshthemes/themes.zip -d ~/.poshthemes
chmod u+rw ~/.poshthemes/*.json
rm ~/.poshthemes/themes.zip
```
2. Elejir tema (Colocar comando en la consola)
```
eval "$(oh-my-posh --init --shell bash --config ~/.poshthemes/<nombre-del-tema>.omp.json)"
```
3. guardar tema una vez ya has elejido el que te guste
```
nano .bashrc
```
ir al final de el archivo colocar la linia de codigo y guardar `(ctrl+o, enter, ctrl+x)`
```
#themes oh-my-posh
eval "$(oh-my-posh --init --shell bash --config ~/.poshthemes/<nombre-del-tema>.omp.json)"
```
4. actualizar el bashrc
```
source .bashrc
```


