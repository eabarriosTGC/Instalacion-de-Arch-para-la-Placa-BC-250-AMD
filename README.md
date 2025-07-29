# Instalacion de Arch Linux para la Placa BC-250 AMD
Guía paso a paso para instalar una versión base de Arch Linux en la placa de minería AMD BC-250. Estas placas, diseñadas originalmente para criptominería, son un hardware peculiar pero funcional que puede ser reutilizado como un PC GAMER.

---

## ⚠️ Advertencia

Este proceso implica formatear el disco de almacenamiento de la placa. Realiza una copia de seguridad de cualquier dato importante antes de comenzar. Sigue esta guía bajo tu propio riesgo.

---

## Requisitos Previos

Antes de empezar, asegúrate de tener lo siguiente:
*   Una placa BC-250.
*   Unidad USB de al menos 4 GB.
*   La imagen ISO oficial de Arch Linux (puedes descargarla [aquí](https://archlinux.org/download/)).
*   Un ordenador para preparar la unidad USB de arranque.
*   Software para "flashear" la ISO en el USB (como [BalenaEtcher](https://www.balena.io/etcher/) o [Rufus](https://rufus.ie/)).
*   Conexión a internet por cable Ethernet para la placa.

### Paso 2: Configuración Inicial
Al iniciar ingresamos el siguiente comando y le damos enter:
  archinstall
![Image alt](https://github.com/eabarriosTGC/Instalacion-de-Arch-para-la-Placa-BC-250-AMD/blob/bdc0ceb855f6f98c08cf940a51821d052be020b2/archinstall.png)



### Se cargara el siguiente menu para ayudarnos en la instalacion y eligen en la primera opcion el idioma que prefieran.
![Image alt](https://github.com/eabarriosTGC/Instalacion-de-Arch-para-la-Placa-BC-250-AMD/blob/bdc0ceb855f6f98c08cf940a51821d052be020b2/menu-Archinstall.png)


### EN LA OPCIONES DE LOCALIDADES ELIGEN EL IDIOMA Y EL TIPO DE TECLADO QUE PREFIERAN.
![Image alt](https://github.com/eabarriosTGC/Instalacion-de-Arch-para-la-Placa-BC-250-AMD/blob/bdc0ceb855f6f98c08cf940a51821d052be020b2/Localidades.png)


### EN LA OPCION DE MIRRORS Y REPOSITORIOS ELIGEN LAS REGIONES CANADA Y UNITED STATES(PARA SELECCIONAR ES CON LA TECLA ESPACIO) Y EN LA OPCIONES DE REPOSITORIOS ELIGEN LOS DOS QUE SALEN CON LA TECLA ESPACIO.
![Image alt](https://github.com/eabarriosTGC/Instalacion-de-Arch-para-la-Placa-BC-250-AMD/blob/bdc0ceb855f6f98c08cf940a51821d052be020b2/regiones.png)
![Image alt](https://github.com/eabarriosTGC/Instalacion-de-Arch-para-la-Placa-BC-250-AMD/blob/bdc0ceb855f6f98c08cf940a51821d052be020b2/repo-Adicionales.png)



### EN LA OPCION DE CONFIGURACION ELIGEN SU UNIDAD DE ALMACENAMIENTO Y ELIGEN LA OPCION DE MEJOR ESFUERZO CON FORMATO EXT4, SI SALE SALE EL AVISO DE CREAR UNA CARPETA /HOME SEPARADA LE DAN LA OPCION NO.
![Image alt](https://github.com/eabarriosTGC/Instalacion-de-Arch-para-la-Placa-BC-250-AMD/blob/bdc0ceb855f6f98c08cf940a51821d052be020b2/particionamiento.png)
![Image alt](https://github.com/eabarriosTGC/Instalacion-de-Arch-para-la-Placa-BC-250-AMD/blob/bdc0ceb855f6f98c08cf940a51821d052be020b2/ext4.png)


### EN LA OPCION DE SWAP LA DEJAN HABILITADA.
![Image alt](https://github.com/eabarriosTGC/Instalacion-de-Arch-para-la-Placa-BC-250-AMD/blob/bdc0ceb855f6f98c08cf940a51821d052be020b2/zram.png)


### EN LA OPCION DE GESTOR DE ARRANQUE ELIGEN GRUB.
![Image alt](https://github.com/eabarriosTGC/Instalacion-de-Arch-para-la-Placa-BC-250-AMD/blob/bdc0ceb855f6f98c08cf940a51821d052be020b2/grub.png)


### EN LA LAS SIGUIENTES OPCIONES CREAN UNA CONTRASEÑA ROOT, CREAN UN USUARIO Y CONTRASEÑA CON PERMISOS ROOT.
![Image alt](https://github.com/eabarriosTGC/Instalacion-de-Arch-para-la-Placa-BC-250-AMD/blob/bdc0ceb855f6f98c08cf940a51821d052be020b2/usuario.png)
![Image alt](https://github.com/eabarriosTGC/Instalacion-de-Arch-para-la-Placa-BC-250-AMD/blob/bdc0ceb855f6f98c08cf940a51821d052be020b2/confirmarYsalir.png)


### EN LA OPCION DE PERFIL ELIGEN DESKTOP Y EL ESCRITORIO GNOME (PUEDEN ELEGIR EL QUE PREFIERAN).
![Image alt](https://github.com/eabarriosTGC/Instalacion-de-Arch-para-la-Placa-BC-250-AMD/blob/bdc0ceb855f6f98c08cf940a51821d052be020b2/Perfil-Destokp.png)
![Image alt](https://github.com/eabarriosTGC/Instalacion-de-Arch-para-la-Placa-BC-250-AMD/blob/main/gnome.png)

### EN LA OPCION DE CONTROLADORES GRAFICOS ELIGEN EL DE AMD/ATI (OPEN SOURCE)
![Image alt](https://github.com/eabarriosTGC/Instalacion-de-Arch-para-la-Placa-BC-250-AMD/blob/bdc0ceb855f6f98c08cf940a51821d052be020b2/Controladores-Amd.png)


### EN LA OPCION DE AUDIO PUEDEN ELEGIR EL DE SU PREFERECIA(EN ESTE CASO ELEGIMOS PIPEWIRE)
![Image alt](https://github.com/eabarriosTGC/Instalacion-de-Arch-para-la-Placa-BC-250-AMD/blob/bdc0ceb855f6f98c08cf940a51821d052be020b2/audio.png)


### EN LA OPCION DE NUCLEO DESMARCAMOS CON LA TECLA ESPACION EL PREDETERMINADO Y ELEGIMOS EL LTS.(Actualmente el kernel 6.15.8 ya no presenta problemas de congelamiento de pantalla)
![Image alt](https://github.com/eabarriosTGC/Instalacion-de-Arch-para-la-Placa-BC-250-AMD/blob/bdc0ceb855f6f98c08cf940a51821d052be020b2/nucleoLts.png)


### POR ULTIMO EN LA OPCION DE CONFIGURACION DE RED ELEGIMOS LA NETWORKMANAGER
![Image alt](https://github.com/eabarriosTGC/Instalacion-de-Arch-para-la-Placa-BC-250-AMD/blob/bdc0ceb855f6f98c08cf940a51821d052be020b2/configuracionRed.png)



### LLE DAN INSTALAR Y LUEGO CONFIRMAN. PARA INSTALAR LA CONFIGURACION PARA GARANTIZAR EL FUNCIONAMIENTO PARA GAMING Y PROGRAMAS FLATPAK SIGUEN DESPUES ESTE TUTORIAL:
https://github.com/eabarriosTGC/BC250--ARCH


