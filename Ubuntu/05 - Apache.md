# 05 - Instalación de Apache en Ubuntu

Actualizamos la lista de repositorios:

```bash
sudo apt update
```

Instalamos `Apache 2`:

```bash
sudo apt -y install apache2 apache2-utils
```

Agregamos compatibilidad con `PHP 8.1` instalando el siguiente módulo:

```bash
sudo apt -y install libapache2-mod-php8.1
```

Reiniciamos el servicio de `Apache 2`:

```bash
sudo systemctl restart apache2
```
