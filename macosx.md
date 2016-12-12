# Instalación en Mac OSX

Para instalar Ruby en Mac necesitas tener instalado [Homebrew](http://brew.sh/) primero.

## Homebrew

Para verificar si ya lo tienes instalado abre una **Terminal** y ejecuta lo siguiente:

```
$ brew -v
```

Si te dice que el comando no fue encontrado debes instalar [Homebrew](http://brew.sh/) primero. Para eso ejecuta el siguiente comando en la **Terminal**:

```
$ ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

Cuando te pida instalar las herramientas de la línea de comandos de XCode, acepta.

## Ruby

Para instalar Ruby vamos a utilizar un manejador de paquetes llamado rbenv que te va a permitir tener varias versiones de Ruby instaladas de forma simultánea.

Para instalar rbenv y Ruby ejecuta los siguientes comandos:

```
brew install rbenv ruby-build

# Add rbenv to bash so that it loads every time you open a terminal
echo 'if which rbenv > /dev/null; then eval "$(rbenv init -)"; fi' >> ~/.bash_profile
source ~/.bash_profile

# Install Ruby
rbenv install 2.3.1
rbenv global 2.3.1
ruby -v
```

Al ejecutar el último comando deberías ver la versión de Ruby que acabas de instalar.

Si tienes problemas instalando Ruby y eres alumno de Make it Real contacta a tu mentor para que te ayude a revisar.
