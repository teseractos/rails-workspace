Ruby on Rails workspace
=========

Configuraci�n de m�quina virtual con Ruby 2.1.1 y Rails 4.

El puerto 3000 (puerto por defecto de Rails) en el equipo host est� redirigido al puerto 3000 en la m�quina virtual.

## Requisitos

* [VirtualBox](https://www.virtualbox.org)

* [Vagrant](http://vagrantup.com)

## Qu� contiene la m�quina virtual

* Git

* Ruby 2.1.1

* Node.js

* Rails 4.1.0

* PostgreSQL

## C�mo construir la m�quina virtual

Para levantar la m�quina solo hay que hacer lo siguiente:

    git clone https://github.com/teseractos/rails-workspace.git
    cd rails-workspace
    vagrant up

Una vez la instalaci�n ha finalizado, se puede acceder a la m�quina virtual con

    vagrant ssh

o simplement utilizando cualquier cliente ssh con el usuario _vagrant_ y la contrase�a _vagrant_.

Si se emplea la VM detr�s de un proxy es necesario instalar el plugin proxyconf y descomentar la configuraci�n del proxy en el Vagrantfile.

    vagrant plugin install vagrant-proxyconf

Por defecto, el directorio rails-workspace (el que contiene el Vagrantfile) est� sincronizado con el directorio /vagrant en la m�quina virtual.

Por favir, revisa la [documentaci�n de Vagrant](http://docs.vagrantup.com/v2/) para m�s informaci�n.