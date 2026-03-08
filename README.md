# Proyecto: Servidor Linux con SSH y gestión de usuarios

## Objetivo
Configurar un servidor Linux seguro con acceso remoto por SSH, gestión de usuarios, grupos y permisos.

## Tecnologías utilizadas
- Ubuntu Server
- OpenSSH
- Gestión de usuarios y grupos
- Permisos de archivos y carpetas
- Autenticación mediante claves SSH

## Funcionalidades implementadas
- Creación de varios usuarios
- Creación de grupos
- Configuración de permisos en carpetas
- Acceso remoto por SSH
- Desactivación del login de root
- Configuración de autenticación con claves SSH

## Comandos principales

### Instalar SSH
```bash
sudo apt update
sudo apt install openssh-server -y
```

### Crear usuarios
```bash
sudo adduser juan
sudo adduser maria
sudo adduser devops
```

### Crear grupos
```bash
sudo groupadd developers
sudo groupadd admins
```

### Añadir usuarios a grupos
```bash
sudo usermod -aG developers juan
sudo usermod -aG developers maria
sudo usermod -aG admins devops
```

### Crear carpeta de proyecto
```bash
sudo mkdir -p /proyectos/app1
sudo chown :developers /proyectos/app1
sudo chmod 770 /proyectos/app1
```

## Configuración de seguridad
- Se desactivó el acceso SSH directo del usuario root.
- Se configuró autenticación por clave SSH.
- Se ajustaron permisos para limitar el acceso según grupo.

## Aprendizajes
Con este proyecto he practicado:
- Administración básica en Linux
- Gestión de usuarios y grupos
- Permisos
- Acceso remoto seguro
- Seguridad básica en servidores

## Autor
Hugo