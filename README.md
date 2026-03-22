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

### Permisos

## 3. Software esencial



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

## 9. Gestión de energia (para portatiles)

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
