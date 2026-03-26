![Ubuntu](https://img.shields.io/badge/Ubuntu-24.04-orange)
![Estado](https://img.shields.io/badge/estado-en%20progreso-yellow)
# Ubuntu después de la instalación
> **Nota:** Todavía no está acabada la guía.

Esto es una guía con programas que instalar, configuraciones, wallpapers, enlaces de interés, entre otras cosas para _Ubuntu 24.04 LTS_.

## Índice

- [1. Preparacion inicial](#1-preparacion-inicial)
- [2. Seguridad basica](#2-seguridad-basica)
- [3. Software esencial](#3-software-esencial)
- [4. Herramientas de desarrollo](#4-herramientas-de-desarrollo)
- [5. Virtualizacion y contenedores](#5-virtualizacion-y-contenedores)
- [6. Gestion de paquetes](#6-gestion-de-paquetes)
- [7. Personalizacion del sistema](#7-personalizacion-del-sistema)
- [8. Optimizacion y rendimiento](#8-optimizacion-y-rendimiento)
- [9. Gestión de energia (para portatiles)](#9-gestion-de-energia-para-portatiles)
- [10. Gaming](#10-gaming)
- [11. Copias de seguridad](#11-copias-de-seguridad)
- [12. Automatizacion y scripts](#12-automatizacion-y-scripts)
- [13. Consejos y trucos](#13-consejos-y-trucos)
- [14. Solucion de problemas](#14-solucion-de-problemas)

## 1. Preparacion inicial
Antes de tocar algo en el sistema, siempre es buena idea actualizar los repositorios.

```bash
sudo apt update && sudo apt upgrade -y
```
## 2. Seguridad basica

### Contraseñas

- Usar contraseñas complejas y únicas, no usar la misma para tu usuario normal y para root.
- Si tienes la misma contraseña para todas tus cuentas y servicios, un data breach puede arrasar con todo.
- Evitar iniciar sesión en Ubuntu como usuario root, usar sudo siempre que se pueda.

[Enlace](https://www.pluralsight.com/resources/blog/cybersecurity/modern-password-guidelines) a un artículo sobre buenas practicas para contraseñas.

Algunos gestores de contraseña recomendados son Keepass y Bitwarden, que además son de codigo abierto.

### Cifrado

Veracrypt

### Firewall (ufw)
Instalar Uncomplicated Firewall si no lo tienes:
```bash
sudo apt install ufw
```

Activar el firewall:
```bash
sudo ufw enable
sudo ufw status
```
Configuración recomendada:
```bash
sudo ufw limit 22/tcp
sudo ufw allow 80/tcp
sudo ufw allow 443/tcp
sudo ufw default deny incoming
sudo ufw default allow outgoing
sudo ufw enable
```
### Actualizaciones automáticas

### VPN Gratuita

Proton vpn
mullvad vpn

### Permisos

Conguración > Notificaciones y desactivar Lock screen notifications para evitar que nadie vea nada con tu dispositivo debloqueado

### DNS

DNS es esencial para conectarse a Internet, la mayoría de DNS por defecto trakean navegacion. Si usas una vpn probablemente esta ya utiliza su propio DNS
En caso contrario algunos DNS recomendados son 1.1.1.1 y 9.9.9.9
Para mas info ver https://www.privacytools.io/encrypted-dns

## 3. Software esencial

### Navegador

Simplemente evita Chrome. Algunos recomendados son Firefox (con hardening), Librewolf, Mullvad...
Para motor de búsqueda duckduckgo o startpage
### otras cosas (buscar más)
balenaEtcher para hacer usb's bootables, el disks no me funcionó.

instalar curl

antivirus ClamAV

veracrypt para cifrar

sudo apt install libreoffice -y

instalar pip pip3 o pipx

Tambien como consejo general usar FOSS (free and open source software)

## 4. Herramientas de desarrollo

### Git 
Sofware de control de versiones
```bash
sudo apt install git -y
git config --global user.name "TuNombre"
git config --global user.email "tu@email.com"
```

## 5. Virtualizacion y contenedores

Virtualbox de su página oficial

### Docker
```bash
sudo apt install docker.io -y
sudo systemctl enable docker
``` 
Pro tip:
```bash
# Añadiendo esto no necesitas usar siempre sudo
sudo usermod -aG docker $USER
```
## 6. Gestion de paquetes

## 7. Personalizacion del sistema

### Temas

### Íconos

### GNOME Tweaks

### Wallpapers

## 8. Optimizacion y rendimiento

### Limpieza del sistema
```bash
sudo apt autoremove -y
sudo apt autoclean
```
### Servicios innecesarios

## 9. Gestion de energia (para portatiles)

> Tip: Usa temas oscuros para ahorrar batería en portátiles.

## 10. Gaming

### Drivers gráficos

### Steam / Proton

## 11. Copias de seguridad



## 12. Automatizacion y scripts



## 13. Consejos y trucos

## 14. Solucion de problemas

## Contribuciones

Todas las contribuciones para mejorar esta guía son bienvenidas. Abre un issue o pull request.
