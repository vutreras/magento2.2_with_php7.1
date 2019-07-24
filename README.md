#  Magento 2 Docker para desarrollo

### Apache 2.4 + PHP 7.1 + MariaDB

## Requerimientos

**MacOS:**

Instalar [Docker](https://docs.docker.com/docker-for-mac/install/), [Docker-compose](https://docs.docker.com/compose/install/#install-compose)

**Windows:**

Instalar [Docker](https://docs.docker.com/docker-for-windows/install/), [Docker-compose](https://docs.docker.com/compose/install/#install-compose)

**Linux:**

Instalar [Docker](https://docs.docker.com/engine/installation/linux/docker-ce/ubuntu/) y [Docker-compose](https://docs.docker.com/compose/install/#install-compose).

### Como usar

De forma automática se creará una imagen Prestashop con una tienda de pruebas

Para instalar Magento 2, hacer lo siguiente:

### Construir el contenedor desde cero

```
./docker-build.sh
```

### Iniciar el contenedor construido anteriormente

```
./docker-start.sh
```

### Acceder al contenedor

```
./docker-shell.sh
```

### Paneles

Web server: http://localhost/  
Admin: http://localhost/admin  
PHPMyAdmin: http://localhost:8090  
- user: admin
- password: admin123 

**Cuenta**

Además debes tener o crear una cuenta en Magento Marketplace siguiendo este tutorial oficial: [https://devdocs.magento.com/guides/v2.2/install-gde/prereq/connect-auth.html](https://devdocs.magento.com/guides/v2.2/install-gde/prereq/connect-auth.html)

Luego de crear la cuenta y crear la llave de acceso debes respaldar "Public Key" y "Private Key" dado que pueden ser requeridas durante el proceso de instalación de magento2.

## Instalación y/o ejecución

### Como instalar magento2

Para instalar Magento 2, hacer lo siguiente:

Además se puede especificar la versión a instalar (e.j. `install-magento2 2.2.6`).

```
./docker-build.sh
install-magento2 2.2.6
```

### Licencia

MIT © 2018

Basado en: [Rafael Corrêa Gomes](https://github.com/rafaelstz/) and [contributors](https://github.com/clean-docker/Magento2/graphs/contributors).
