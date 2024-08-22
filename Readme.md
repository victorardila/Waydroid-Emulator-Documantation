# Instalación y ejecución de Waydroid en Linux

<p align="center">
  <img src="https://github.com/user-attachments/assets/f51f1f07-29d8-41c8-8f55-dd4649386f95" alt="waydroid_logo" />
</p>

## Instalacion en Linux

## `Ubuntu linux y cualquiera de sus derivados`
Para ejecutar de forma grafica waydroid es decir el emulador debe descargar un compositor de ventanas wayland para este caso se usara `Weston` lo puedes instalar con el siguiente comando:

```diff
sudo apt install weston
```

### - Ejecutar el servicio de waydroid
```diff
waydroid session start
```
### - DEtener el servicio de waydroid
```diff
waydroid session stop
```
