# ISéneca: Interfaz de usuario que se complementa con el proyecto de TimeTable o Horarios

# Descripción del proyecto

ISéneca es la interfaz de usuario para gestionar las incidencias que cometen los alumnos fácilmente con una interfaz sencilla y amigable, funciona con el proyecto TimeTable que le manda los datos de alumnos, profesores y horarios que la interfaz recoge y muestra para que los profesores puedan gestionar las incidencias fácilmente, está hecho en el framework de flutter y se conecta con firebase para un loggin sencillo para que los profesores accedan fácilmente

# Instalación de flutter

Instalar y configurar flutter es complicado ya que se necesitan muchos componentes para que el proyecto funcione, lo primero es descargar el [sdk de flutter](https://storage.googleapis.com/flutter_infra_release/releases/stable/windows/flutter_windows_3.19.3-stable.zip) (actualmente es la versión 3.19.3). Una vez que se haya descargado creamos una carpeta <b>src</b> a la altura de C:\ o si es un ordenador compartido a la altura del usuario <b>NUNCA</b> a la altura de los archivos del programa ya que es posible que aparezcan errores de compilación a la hora de ejecutar un proyecto de flutter, cuando hayamos creado la carpeta descomprimimos el zip de flutter dentro de src

Una vez que se haya descomprimido la carpeta en su sitio correspondiente tenemos que acceder a las variables de entorno colocando en el buscador de windows <b>Editar las variables de entorno de esta cuenta</b> buscamos la variable Path y seleccionamos editar, y añadimos esta expresion 

<h3>Si la carpeta está colocada en C:\</h3>

```
C:\src\flutter\bin
```

<h3>Si la carpeta está colocada a la altura del usuario</h3>

```
%USERPROFILE%\src\flutter\bin
```

Para comprobar que flutter se ha instalado aplicamos ```Windows``` + ```R``` y escribimos cmd, cuando se abra el símbolo del sistema escribimos:

```
flutter --version
```

Si aparece que el comando no se encuentra hay un error en la configuración de las variables de entorno, si no mostrará un cuadro de texto y la extensión, si está instalado ejecutaremos el siguiente comando que nos ayudará a validar todos los componentes del entorno de desarrollo de Flutter para Windows:

```
flutter doctor
```

Al principio tardará bastante en ejecutarse pero nos mostrará los requisitos para ejecutarlo. Un ejemplo de ello es el siguiente:

```
Doctor summary (to see all details, run flutter doctor -v):
[√] Flutter (Channel stable, 3.19.3, on Microsoft Windows [Versi¢n 10.0.22631.3155], locale es-ES)
[√] Windows Version (Installed version of Windows is version 10 or higher)
[!] Visual Studio - develop Windows apps (Visual Studio Build Tools 2019 16.11.32)
    X The current Visual Studio installation is incomplete.
      Please use Visual Studio Installer to complete the installation or reinstall Visual Studio.
[!] Android Studio (not installed)
[X] Android toolchain - develop for Android devices
    X Unable to locate Android SDK.
      Install Android Studio from: https://developer.android.com/studio/index.html
      On first launch it will assist you in installing the Android SDK components.
      (or visit https://flutter.dev/docs/get-started/install/windows#android-setup for detailed instructions).
      If the Android SDK has been installed to a custom location, please use
      `flutter config --android-sdk` to update to that location.

[√] Chrome - develop for the web
[√] VS Code (version 1.86.2)
[√] Connected device (3 available)
[√] Network resources

! Doctor found issues in 3 categories.
```

El primero de ellos es tener Visual Studio Code instalado para programar y arrancar flutter para instalarlo accedemos al [enlace de descarga](https://code.visualstudio.com/download) y seleccionamos el sistema operativo en el que queremos que se instale

Lo segundo que debemos de tener es Android Studio, un requisito que necesita flutter es una sdk de android studio que necesita flutter para funcionar, lo primero es acceder al [enlace de descarga](https://developer.android.com/studio?hl=es-419) y descargar la ultima version de android studio, cuando se instale y accedamos al menu principal en la esquina superior derecha aparecerán 3 puntos verticales los seleccionamos y seleccionamos <b>Sdk Manager</b> seleccionamos <b>SDK Tools</b> y tenemos que instalar:

<ul>
    <li>Android SDK Command-line Tools (latest)</li>
    <li>Android SDK Platform-Tools</li>
    <li>Google USB Driver</li>
    <li>Android Emulator</li>
    <li>Android Emulator hypervisor driver (installer)</li>
</ul>

Es posible que debido al avance de versiones del IDE algunos sdk vengan instalados por defecto, en ese caso los dejamos instalados

Realizamos de nuevo flutter doctor y aceptamos las licencias de los sdk de android

Debemos de tener instalado Chrome para que flutter se ejecute en la web

Por último accedemos a Visual Studio Code e instalamos las siguientes extensiones

<ul>
<li>Flutter</li>
<li>Dart</li>
<li>Pubspec Assist</li>
</ul>

Una vez con todo instalado podemos arrancar el proyecto, para arrancarlo es muy sencillo solo tenemos que ejecutarlo desde Visual Studio Code y seleccionar como navegador predeterminado Chrome 

# Créditos

Este proyecto ha sido diseñado por los alumnos de 2 DAM supervisado por el profesor Rafael Delgado Cubillas y Francisco Benitez Chico

- [Rafael Delgado Cubillas](https://www.linkedin.com/in/rafael-delgado-cubilla-7034a247/)

- [Francisco Benítez Chico](https://www.linkedin.com/in/franciscobenitezchico/)
