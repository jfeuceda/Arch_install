# ArchLinux-Install

Asissted instalation for ArchLinux.

## Pasos a seguir:

Una vez que iniciado el boot de ArchLinux y se le muestra en el prompt `root@archiso ~ # _`

ejecute los siguientes comandos en el orden solicitado:

- `pacman -Syy`
- `pacman -S git` ( si este le muestra error, volver a ejecutarlo)
- `git clone https://github.com/SolimanHub/arch`
- `cd arch`
- `./main` (T = este tomará tiempo)
- Se le pregunta si desea particionar el disco de forma manual, escriba 's' para si ó 'n' para no (se recomienda 'n' para maquinas virtuales)
- Se le muestran los discos disponibles, seleccione uno escribiendo el nombre especifico de la unidad `sdX` ( ejem `sda` )

    Se crearan 4 particiones raiz, home, EFI y una particion de 1M para la bios

- `./conf` (T)
- Introduzca la contraseña del usuario root
- Introduzca nombre del nuevo usuario no root
- Introduzca la contraseña del usuario no root
- `./user_conf`
- `exit`
- `exit`
- `reboot` en caso de no reiniciar, volver a ejecutar `exit` -> `reboot`
