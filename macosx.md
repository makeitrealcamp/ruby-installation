# Instalación en Mac OSX

Para instalar Ruby vamos a utilizar un manejador de paquetes llamado [rvm](https://rvm.io/) que te va a permitir tener varias versiones de Ruby instaladas en tu máquina.

Para instalar `rvm` y Ruby ejecuta los siguientes comandos:

```
sudo apt-get install libgdbm-dev libncurses5-dev automake libtool bison libffi-dev
gpg --keyserver hkp://keys.gnupg.net --recv-keys 409B6B1796C275462A1703113804BB82D39DC0E3
curl -sSL https://get.rvm.io | bash -s stable
source ~/.rvm/scripts/rvm
rvm install 2.3.3
rvm use 2.3.3 --default
ruby -v
```

Al ejecutar el último comando deberías ver la versión de Ruby que acabas de instalar.

Si tienes problemas instalando Ruby y eres alumno de Make it Real contacta a tu mentor para que te ayude a revisar.
