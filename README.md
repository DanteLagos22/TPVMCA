# TPVMCA
Trabajo practico final de Computacion Aplicada

###  Alumnos:

**Dante Thomas Lagos**

**Sergio Emiliano Barrios**

**Cristhoper Segovia**

**Juan Ignacio Paracchini**



# Configuracion GNU/Linux sabor Debian
# Automatizacion de Backup con scripts



## Requisitos

- Debian GNU/Linux (Sin entorno grafico o GUI)
- VirtualBox
- Acceso SSH

## Contenido:
#### Este repositorio contiene la configuracion y scripts desarrollados para el Trabajo Practico grupal Final, Incluye:

- /root (configuración de claves)
- /etc (archivos del sistema y configuración de servicios)
- /opt/scripts (script de backup automatizado)
- /proc/particion (archivo simulado de particiones) (El original no se puede exportar)
- /www_dir (contenido del sitio web)
- /backup_dir (backups generados)
- /var (dividido en partes por tamaño)

## Servicios Configurados

- **Red**: interfaz estática `192.168.1.100`.
- **SSH**: habilitado con autenticación por clave pública/privada.
- **Apache2**: servidor web configurado para servir archivos desde `/www_dir`.
- **PHP 7.3**: instalado y habilitado para ejecución en Apache.
- **Discos adicionales**: se crearon y montaron particiones dedicadas a `/www_dir` y `/backup_dir`.
- **Backup**: script automatizado `backup_full.sh` ejecutado por cron según cronograma.

## Automatización de Tareas

- Backup diario de `/var/log` a las 00:00 h.
- Backup de `/www_dir` los lunes, miércoles y viernes a las 23:00 h.
- Script con validaciones y logs, ubicado en `/opt/scripts`.



### Fin
##### Que la fuerza los acompañe
