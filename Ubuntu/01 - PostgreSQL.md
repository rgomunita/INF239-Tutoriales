# 01 - Instalación de PostgreSQL en Ubuntu

Actualizamos la lista de repositorios:

```bash
sudo apt update
```

Añadimos la clave pública del repositorio de `PostgreSQL`:

```bash
wget --quiet -O - https://www.postgresql.org/media/keys/ACCC4CF8.asc | sudo apt-key add -
```

Añadimos el repositorio de `PostgreSQL`:

```bash
echo "deb [arch=amd64] http://apt.postgresql.org/pub/repos/apt/ `lsb_release -cs`-pgdg main" | sudo tee  /etc/apt/sources.list.d/pgdg.list
```

Actualizamos nuevamente la lista de repositorios:

```bash
sudo apt update
```

Instalamos `PostgreSQL`:

```bash
sudo apt install postgresql-14 postgresql-client-14
```

Iniciamos sesión con el usuario `postgres`:

```bash
sudo su - postgres
```

Comprobamos el estado del servicio de `PostgreSQL`:

```bash
systemctl status postgresql.service 
```

Cambiamos la contraseña del usuario `postgres`:

```bash
psql -c "alter user postgres with password 'ContraseñaSuperFuerte'"
```
