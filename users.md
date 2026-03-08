# Gestión de usuarios y grupos

## Usuarios creados
- juan
- maria
- devops

## Grupos creados
- developers
- admins

## Comandos utilizados

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

## Objetivo
Separar usuarios por funciones y gestionar mejor los permisos mediante grupos.