# Proyecto-qr-duoc
 proyecto creado con ionic y angular que marca la asistencia de un estudiante mediante codigo qr
# Intalaciones requeridas:
 ```bash
 -Node.js
 ```
 ```bash
 -Java jdk 8
 ```
 ```bash
 -Android Studio
 ```
# pasos que se usaron para crear la app en ionic
```bash
crear carpeta para el proyecto
```
```bash
 abrir consola como admin y abrir carpeta del proyecto en la consola
 ```
 ```bash
ejecutar este comando npm install -g @ionic/cli
```
este comando  hara que node instale globalmente  las lineas de comando de ionic
```bash
ionic start app-register blank
```
ejecutar este comando para crear nuestra aplicacion en ionic
```bash
le pedira que framework utilizar en este caso se utilizo angular
```
```
ejecutar comando ionic serve si quiere correr el servidor de la app y ctrl + c para cerrar servidor
```
```bash
abrir windows powershell como admin y ejecutar este comando Set-ExecutionPolicy Unrestricted
```
este comando es opcional si esque no se puede ejecutar scripts
```bash 
# ionic g page pages/login
```
con este comando vamos a poder crear paginas en ionic
 # para poder usar imagenes seguir los siguientes pasos
```bash
para usar imagenes en la app descarguela en formato svg
```
```bash
dentro de la carpeta assets crear una carpeta llamada images
```
```bash
colocar la imagen dentro de esa carpeta
```
```bash
<ion-img src="assets/images/nombre-img.svg">
```
 ejemplo de como usar la imagen
  
# para proteger la ruta de la app y no saltarse el login se hara uso del siguiente comando
```bash
ionic g service services/Autenticacion
```
en este archivo se le dara seguridad a las rutas para que no se puedan acceder a ella mediante url

# para poder Instalar dos nuevas variables de entorno seguir los siguientes pasos
```bash
ir a opciones avanzadas y crear nueva variable de entorno poner de nombre JAVA_HOME y en valor darle la ruta del jdk que descargo
```
```bash
crear otra variable darle el nombre de ANDROID_SDK-ROOT y su valor sera usuario/user/AppData/local/android/sdk
```

  
# Android
para poder usar android nativo ejecutar los siguientes comandos
```bash
ionic build
```
este comando se encarga de paquetizar tu producto para ser finalmente exportado
```bash
npm install @capacitor/android 
```
instala el capacitor de android
```bash  
npx cap add android
```
con este comando el capacitor agrega el proyecto android
```bash
ionic cap run android --livereload --external
```
con este comando correremos la app de forma nativa en un emulador de android studio o si tiene un celular android en modo desarrollador conectado por usb 

# sqlite
para poder usar sqlite en la app son necesarios estos comandos
```bash  
npm install cordova-sqlite-storage
```
este comando prepara la app para que tenga almacenamiento propio de sqlite
```bash
npm install @ionic-native/core
```
este comando nos permite acceder a los recursos nativos del telefono
```bash
npm install @ionic-native/sqlite
```
```bash
ionic cap sync
```
este comando va a tomar las instalaciones previas las va a paquetizar, para que se comporten como una unica unidad
  
  
# QR
para poder usar la camara del dispositivo dentro de la app ya sea en emulador o celular por cable usb hay que ejecutar estos comandos
```bash
npm install @capacitor/camera
```
```bash
npm install @ionic-native/core
```
```bash
ionic cap sync
```
```bash
ir a la carpeta de android  y añadir los permisos correspondientes
```
