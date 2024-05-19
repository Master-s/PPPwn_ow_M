# PPPwn_OpenWrt
He añadido una interfaz web para arrancar PPPwn_cpp desde un teléfono solamente conectandote al router.
Descarga la ultima version [descargar pppwn_cpp repositorio oficial](https://nightly.link/xfangfang/PPPwn_cpp/workflows/ci.yaml/main).

## Requerimientos:

- Router/Modem conexión lan con OpenWrt.
- Tener instalado PuTTY en tu PC para acceder por el terminal.
- Descargar stage1.bin y stage2.bin desde el repositorio de Stooged para el firmware correspondiente.
- Descargar PPPwn_cpp para distribuciones Linux con chip MIPS o el que tu dispositivo tenga, verificar con el comando `uname -m`.
- Descargar goldhen.bin para el Firmware de tu consola.

## Instalación

1. Desde el terminal en su router, ejecuta el comando `cd `
2. Después, ejecuta el comando `wget https://github.com/CodeInvers3/PPPwn_ow/archive/refs/heads/main.zip`
3. Ejecuta el comando `unzip main`, luego ejecuta el comando `chmod +x PPPwn_ow-main/install.sh`
4. Por último, ejecuta el comando `PPPwn_ow-main/install.sh`
5. Verifica qué chip tiene tu dispositivo router con `uname -m`. De acuerdo a eso, elige cuál ejecutable pppwn debes descargar.
6. Busca el ejecutable pppwn en el [repositorio oficial](https://nightly.link/xfangfang/PPPwn_cpp/workflows/ci.yaml/main)
7. Descarga el repositorio con el comando `wget url_de_tu_pppwn`
8. Descomprime el archivo descargado con `unzip pppwn_archivo.zip` y después bórralo con `pppwn_archivo.zip`
9. Descomprime el archivo `tar -xzvf pppwn.tar.gz` y después bórralo con `rm pppwn.tar.gz`
10. Por último, ejecuta el comando `chmod +x pppwn` y `mv pppwn /usr/bin`
12. Copia goldhen.bin a su memoria usb, debe estar formateada en exFat o FAT32
13. Conectar todo a la consola PS4 y desde el navegador ingresar a la dirección ip de su router (http://192.168.1.1/pppwn.html)

Probado en mini router GL-MT300N-V2 Mango

This is an adaptation of Stooged’s script to work with PPPwn_cpp.

It enables auto-start on a Wi-Fi device running the OpenWrt system.

## Requirements:

- Smart Router lan with OpenWrt.
- Have PuTTY installed on your PC to access the terminal.
- Download stage1.bin and stage2.bin from Stooged’s repository for the corresponding firmware.
- Download PPPwn_cpp for Linux distributions with MIPS chip or whichever your device has, verify with the command `uname -m`.
- Download goldhen.bin for you PS4 FW

## Steps installation:

1. From the terminal on your router, run the command `cd`
2. Then, run the command `wget https://github.com/CodeInvers3/PPPwn_ow/archive/refs/heads/main.zip`
3. Run the command `unzip main`, then run the command `chmod +x PPPwn_ow-main/install.sh`
4. Finally, run the command `PPPwn_ow-main/install.sh`
5. Verify which chip your router device has with `uname -m`. Based on that, choose which pppwn executable you need to download.
6. Look for the pppwn executable in the [official repository](https://nightly.link/xfangfang/PPPwn_cpp/workflows/ci.yaml/main)
7. Download the repository with the command `wget url_of_your_pppwn`
8. Unzip the downloaded file with `unzip pppwn_file.zip` and then delete it with `rm pppwn_file.zip`
9. Extract the file with `tar -xzvf pppwn.tar.gz` and then delete it with `rm pppwn.tar.gz`
10. Finally, run the command `chmod +x pppwn` and `mv pppwn /usr/bin`
12. Copy goldhen.bin to your USB drive; it must be formatted in exFAT or FAT32.
13. Connect everything to the PS4 console and from the browser go to your router's IP address (http://192.168.1.1/pppwn.html)

Every time you turn on the router and connect the USB memory with goldhen.bin, the run.sh script will execute the pppwn command, which will allow the auto-exploit.

PPPwn from https://github.com/xfangfang/PPPwn_cpp

### Credits: Stooged / Xfangfang
