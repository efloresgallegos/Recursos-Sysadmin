# Recursos-Sysadmin


## Comandos generales

Mostrar dispositivos conctados: ```lsblk```

## Redes

Cambiar dirección IP
```
/etc/network/interfaces
```

## Crear Lanzador
Crear lanzador
```
nano /usr/share/applications/Zotero.desktop
```
Escribir el siguiente código en el lanzador:
```
Name=Zotero
Exec=bash -c "$(dirname $(realpath $(echo %k | sed -e 's/^file:\\/\\///')))/zot>
Icon=zotero.ico
Type=Application
Terminal=false
Categories=Office;
MimeType=text/plain;x-scheme-handler/zotero;application/x-research-info-systems>
X-GNOME-SingleWindow=true
```

## Hacer memorias booteables
```
dd if/ruta/imagen.iso of=/dev/sdc status=progress
```

## Kernel

Instalación de headers para virtualizar
1. Verificar version del kernel
´´´ uname -r ´´´
2. Instalar  
´´´apt install linux-headers-$(uname -r)´´´



