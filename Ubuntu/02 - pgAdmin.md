# 02 - Instalación de pgAdmin en Ubuntu

Actualizamos la lista de repositorios:

```bash
sudo apt update
```

Añadimos la clave pública del repositorio de `pgAdmin`:

```bash
wget --quiet -O - https://www.pgadmin.org/static/packages_pgadmin_org.pub | sudo apt-key add -
```

Añadimos el repositorio de `pgAdmin`:

```bash
echo "deb [arch=amd64] https://ftp.postgresql.org/pub/pgadmin/pgadmin4/apt/`lsb_release -cs` pgadmin4 main" | sudo tee /etc/apt/sources.list.d/pgadmin4.list
```

Actualizamos nuevamente la lista de repositorios:

```bash
sudo apt update
```

Instalamos `pgAdmin`:

```bash
sudo apt install pgadmin4
```
