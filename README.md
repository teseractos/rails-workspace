Ruby on Rails workspace
=========

Configuración de máquina virtual con Ruby 2.1.1 y Rails 4.

El puerto 3000 (puerto por defecto de Rails) en el equipo host está redirigido al puerto 3000 en la máquina virtual.

## Requisitos

* [VirtualBox](https://www.virtualbox.org)

* [Vagrant](http://vagrantup.com)

## Qué contiene la máquina virtual

* Git

* Ruby 2.1.1

* Node.js

* Rails 4.1.0

* PostgreSQL

## Cómo construir la máquina virtual

Para levantar la máquina solo hay que hacer lo siguiente:

    git clone https://github.com/teseractos/rails-workspace.git
    cd rails-workspace
    vagrant up

Una vez la instalación ha finalizado, se puede acceder a la máquina virtual con

    vagrant ssh

o simplement utilizando cualquier cliente ssh con el usuario _vagrant_ y la contraseña _vagrant_.

Si se emplea la VM detrás de un proxy es necesario instalar el plugin proxyconf y descomentar la configuración del proxy en el Vagrantfile.

    vagrant plugin install vagrant-proxyconf

Por defecto, el directorio rails-workspace (el que contiene el Vagrantfile) está sincronizado con el directorio /vagrant en la máquina virtual.

Por favir, revisa la [documentación de Vagrant](http://docs.vagrantup.com/v2/) para más información.