# BeEF en Ubuntu 22.04

<p align="center"><img src="https://www.kali.org/tools/beef-xss/images/beef-xss-logo.svg" alt="BeEF Browser Exploit" width="150" height="150"></p>

En este repositorio voy a explicar como instalar BeEF en Ubuntu 22.04.

Lo necesario para llevar a cabo exitosamente la instalación es tener instalado los siguientes paquetes en un sistema operativo Ubuntu 22.04:

* BeEF Browser Exploitation Framework
* ruby
* ruby-dev
* git

## Instalación de ruby y ruby-dev

Para instalar ruby y ruby-dev en ubuntu 22.04, ejecutamos los siguientes comandos:

```bash
sudo apt update
sudo apt install ruby ruby-dev
```

## Instalación de git

Para instalar git en ubuntu 22.04, ejecutamos el siguiente comando:

```bash
sudo apt install git
```

## Clonamos el repositorio de BeEF

Para clonar el repositorio de BeEF, ejecutamos el siguiente comando:

```bash
git clone https://github.com/beefproject/beef.git
```

## Instalamos BeEF

Para instalar BeEF, ejecutamos el siguiente comando:

```bash
cd beef
sudo ./install
```

## Configuramos BeEF

Lo único que tendremos que realizar es configurar unas credenciales más fuertes que las que vienen por default en el archivo de configuración de BeEF, para ello, ejecutamos el siguiente comando:

```bash
nano config.yaml
```

Y en el archivo de configuración, modificamos las siguientes líneas:

```yaml
beef:
  credentials:
    user: "admin"
    pass: "admin"
```

## Iniciamos BeEF

Para iniciar BeEF, ejecutamos el siguiente comando:

```bash
sudo ./beef
```
