# 03 - Instalación de Jupyter Notebook en Ubuntu

Actualizamos la lista de repositorios:

```bash
sudo apt update
```

Instalar `pip3`:

```bash
sudo apt install python3-pip
```

Instalar Jupyter utilizando `pip3`:

```bash
pip3 install jupyter
```

Agregamos `Jupyter` al path, para ello abrimos el archivo `~/.bashrc`:

```bash
sudo nano ~/.bashrc
```

Al final del archivo `~/.bashrc` añadimos la siguiente línea:

```bash
export PATH=$PATH:~/.local/bin
```

Abrimos `Jupyter` con:

```
jupyter notebook
```
