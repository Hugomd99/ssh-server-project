# Permisos de carpetas

## Carpeta creada
`/proyectos/app1`

## Configuración aplicada
```bash
sudo mkdir -p /proyectos/app1
sudo chown :developers /proyectos/app1
sudo chmod 770 /proyectos/app1
```

## Explicación
- El grupo propietario de la carpeta es `developers`.
- El permiso `770` permite acceso completo al propietario y al grupo.
- Los demás usuarios no tienen acceso.

## Objetivo
Restringir el acceso a la carpeta para que solo los usuarios autorizados puedan trabajar en ella.