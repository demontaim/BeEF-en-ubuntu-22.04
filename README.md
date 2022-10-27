# BeEF en ubuntu 22.04

En este repositorio voy a explicar como instalar BeEF en ubuntu 22.04.

Lo necesario para llevar a cabo exitosamente la instalación es tener instalado los siguientes paquetes en un sistema operativo ubuntu 22.04:

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

Para configurar BeEF, ejecutamos el siguiente comando:

```bash