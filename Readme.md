# Instalación y ejecución de Waydroid en Linux

<p align="center">
  <img src="https://github.com/user-attachments/assets/f51f1f07-29d8-41c8-8f55-dd4649386f95" alt="waydroid_logo" />
</p>

## Instalacion en Linux

## `Ubuntu linux y cualquiera de sus derivados`
Para instlar y ejecutar de forma grafica waydroid es decir el emulador debe descargar un compositor de ventanas wayland para este caso se usara `Weston`. La lista de comandos para instalar waydroid es esta:

```diff
# instalacion de waydroid
sudo apt install curl ca-certificates -y
curl https://repo.waydro.id | sudo bash
sudo apt install waydroid -y
# instalacion del compositor
sudo apt install weston
# configuracion de weston
mkdir -p ~/.config/weston
nano ~/.config/weston/weston.ini
```
Esto abrira una ventana de configuracion del sistema. Alli pegaras lo siguiente:

```diff
[core]
# Set the output name
output=HDMI-A-1

[shell]
# Set the default shell
command=weston-terminal
```

### - Ejecutar el servicio de waydroid
```diff
waydroid session start
```
### - DEtener el servicio de waydroid
```diff
waydroid session stop
```
