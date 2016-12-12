# Instalación en Ubuntu

El primer paso para instalar Ruby en Ubuntu es es instalar algunas dependencias con los siguientes comandos:

```
sudo apt-get update
sudo apt-get install git-core curl zlib1g-dev build-essential libssl-dev libreadline-dev libyaml-dev libsqlite3-dev sqlite3 libxml2-dev libxslt1-dev libcurl4-openssl-dev python-software-properties libffi-dev
```

La forma en que recomendamos instalar Ruby es con [rvm](https://rvm.io/). Para hacerlo ejecuta los siguientes comandos:

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

Si te dice que el comando no fue encontrado u algún otro error y eres alumno de Make it Real, contacta a tu mentor para que te ayude a revisar el problema.
