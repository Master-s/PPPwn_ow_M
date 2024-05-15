# PPPwn_ow
Esta es una adaptación del script de Stooged para que funcione con PPPwn_cpp.

Esto permite el autoarranque en un dispositivo con Wi-Fi que utilice el sistema OpenWrt.

## Requerimientos:

- Tener instalado PuTTY en tu PC para acceder por el terminal.
- Descargar stage1.bin y stage2.bin desde el repositorio de Stooged para el firmware correspondiente.
- Descargar PPPwn_cpp para distribuciones Linux con chip MIPS o el que tu dispositivo tenga, verificar con el comando `uname -m`.

## Pasos para el procedimiento:

1. Conectar tu dispositivo a la PC mediante el cable LAN.
2. Configurar el nombre de usuario y contraseña. Si lo requieres, puedes configurar una conexión Wi-Fi en tu dispositivo.
3. Acceder desde el terminal con PuTTY utilizando el comando `ssh usuario@ip_del_router`.
4. Descargar y copiar los archivos run.sh, install.sh, pppwn, stage1.bin y stage2.bin al directorio /root en tu dispositivo con el comando `cp /mnt/usb/* /root`. Esto puedes hacerlo desde tu memoria USB conectándola al dispositivo.
5. Ejecutar install.sh o las líneas de comando contenidas en install.sh.
6. Reiniciar el dispositivo.
  
Cada vez que enciendas el router y conectes la memoria USB con goldhen.bin, el script run.sh ejecutará el comando pppwn, lo que permitirá el autoexploit.

Probado en mini router GL-MT300N-V2 Mango

This is an adaptation of Stooged’s script to work with PPPwn_cpp.

It enables auto-start on a Wi-Fi device running the OpenWrt system.

## Requirements:

- Have PuTTY installed on your PC to access the terminal.
- Download stage1.bin and stage2.bin from Stooged’s repository for the corresponding firmware.
- Download PPPwn_cpp for Linux distributions with MIPS chip or whichever your device has, verify with the command `uname -m`.

## Steps for the procedure:

1. Connect your device to the PC using a LAN cable.
2. Set up the username and password. If required, you can configure a Wi-Fi connection on your device.
3. Access from the terminal with PuTTY using the command `ssh username@router_ip`.
4. Download and copy the files run.sh, install.sh, pppwn, stage1.bin, and stage2.bin to the /root directory on your device with the command `cp /mnt/usb/* /root`. You can do this from your USB memory by connecting it to the device.
5. Execute install.sh or the command lines contained in install.sh.
6. Restart the device.

Every time you turn on the router and connect the USB memory with goldhen.bin, the run.sh script will execute the pppwn command, which will allow the auto-exploit.

Script de https://github.com/stooged/PI-Pwn

PPPwn de https://github.com/xfangfang/PPPwn_cpp

### Credits: Stooged / Xfangfang
