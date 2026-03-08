# Configuración SSH

## Instalación
```bash
sudo apt update
sudo apt install openssh-server -y
```

## Archivo principal de configuración
`/etc/ssh/sshd_config`

## Cambios realizados
```text
PermitRootLogin no
PasswordAuthentication no
```

## Configuración de clave SSH
En el cliente:
```bash
ssh-keygen
ssh-copy-id juan@IP_DEL_SERVIDOR
```

## Objetivo
Aumentar la seguridad del acceso remoto al servidor.