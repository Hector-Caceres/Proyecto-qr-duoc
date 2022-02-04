# Proyecto-qr-duoc
#proyecto creado con ionic y angular que marca la asistencia de un estudiante mediante codigo qr
# Intalaciones requeridas:
 -Node.js
 -Java jdk 8
 -Android Studio
# crear carpeta para el proyecto
# abrir consola como admin y abrir carpeta del proyecto en la consola
# ejecutar este comando npm install -g @ionic/cli
# este comando  hara que node instale globalmente  las lineas de comando de ionic
# ejecutar este comando para crear nuestra aplicacion en ionic
# ionic start app-register blank 
# le pedira que framework utilizar en este caso yo utilize angular 
# ejecutar comando ionic serve si quiere correr el servidor de la app y ctrl + c para cerrar servidor
# abrir windows powershell como admin y ejecutar este comando
# Set-ExecutionPolicy Unrestricted
# este comando es opcional si esque no se puede ejecutar scripts
# con este comando vamos a poder crear paginas en ionic 
# ionic g page pages/login 

# para usar imagenes en la app descarguela en formato svg 
# dentro de la carpeta assets crear una carpeta llamada images
# colocar la imagen dentro de esa carpeta 
# ejemplo de como usar la imagen 
# <ion-img src="assets/images/nombre-img.svg">
  
  
# para proteger la ruta de la app y no saltarse el login se hara uso del siguiente comando
# ionic g service services/Autenticacion
# en este archivo se le dara seguridad a las rutas para que no se puedan acceder a ella mediante url

# Instalar dos nuevas variables de entorno, buscarlas en el buscador de windows
# ir a opciones avanzadas y crear nueva variable de entorno poner de nombre JAVA_HOME y en valor darle la ruta del jdk que descargo
# crear otra variable darle el nombre de ANDROID_SDK-ROOT y su valor sera usuario/user/AppData/local/android/sdk

  
  
# ejecutar comando ionic build 
# este comando se encarga de paquetizar tu producto para ser finalmente exportado

# npm install @capacitor/android 
# instala el capacitor de android
  
# npx cap add android 
# con este comando el capacitor agrega proyecto android

# ionic cap run android --livereload --external
# con este comando correremos la app de forma nativa en un emulador de android studio o si tiene un celular android en modo desarrollador conectado por usb 

# para poder usar sqlite en la app son necesarios estos comandos
  
# npm install cordova-sqlite-storage
  # este comando prepara la app para que tenga almacenamiento propio de sqlite
  
npm install @ionic-native/core
  # este comando nos permite acceder a los recursos nativos del telefono
  
npm install @ionic-native/sqlite
  
ionic cap sync
  # este comando va a tomar las instalaciones previas las va a paquetizar, para que se comporten como una unica unidad
  
  

# para poder usar la camara del dispositivo dentro de la app ya sea en emulador o celular por cable usb hay que ejecutar ciertos comandos
  
  npm install @capacitor/camera
  npm install @ionic-native/core
  ionic cap sync
  ir a la carpeta de android  y añadir los permisos correspondientes

