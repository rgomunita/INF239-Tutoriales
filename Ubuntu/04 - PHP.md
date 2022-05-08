# 04 - Instalación de PHP en Ubuntu

Para poder disfrutar de las últimas versiones de `PHP 8.1` y sus extensiones, añadimos el siguiente repositorio:

```bash
sudo add-apt-repository -y ppa:ondrej/php
```

Actualizamos la lista de repositorios:

```bash
sudo apt update
```

Borramos las versiones anteriores de `PHP`:

```bash
sudo apt -y remove php*
sudo apt -y purge php*
```

Instalamos la base de `PHP 8.1`:

```bash
sudo apt -y install php8.1 php8.1-cgi php8.1-common php8.1-cli php8.1-fpm
```

Instalamos las siguientes extensiones útiles para `PHP 8.1`:

```bash
sudo apt -y install php8.1-opcache php8.1-readline php8.1-zip php8.1-xml php8.1-mbstring php8.1-bcmath php8.1-curl php8.1-gd php8.1-intl php8.1-imagick php8.1-memcached php8.1-soap
```

Instalamos las extensiones de `PHP 8.1` que dan soporte a las bases de datos `MySQL` y `PostgreSQL`:

```bash
sudo apt -y install php8.1-mysql php8.1-pgsql
```