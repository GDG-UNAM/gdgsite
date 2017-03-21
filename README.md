# gdgsite
En este repositorio se encuentra el sitio del GDG UNAM

Despues de clonar el repositorio hay que seguir una serie de pasos para poder correr el projecto:

1.- Instalar firebase CLI (previamente tener instalado npm).
	COMANDO: npm install -g firebase-tools
	Para verificar que todo esta funcionando correctamente poner firebase en la terminal y dar enter.

2.- Login: Ya instalado Firebase CLI debemos acceder con una cuenta 	de google.
	COMANDO: firebase login
	Este comando abrira una ventana en tu navegador solicitando los permisos que Firebase necesita, LA CUENTA TIENE QUE SER LA MISMA QUE SE UTILIZO PARA CREAR EL PROYECTO.

3.- Crear un nuevo proyecto en Firebase 
	LINK: https://firebase.google.com

4.- Vincular el proyecto de Firebase que creamos en el paso 1.
	COMANDO: firebase use --add

5.- En la ruta public/includes/js se debe crear la carpeta keys y 		dentro de ella el archivo firebaseInit.js de modo que la ruta 		quede public/includes/js/keys/firebaseInit.js

6.- En el archivo firebaseInit.js se deben poner las credenciales 		de firebase para web (no se necesitan las etiquetas script ni 		el src a firebase)
	Ejemplo:
	  var config = {
	    apiKey: "YOUR_API_KEY",
	    authDomain: "YOUR_AUTH_DOMAIN",
	    databaseURL: "YOUR_DATABASE_URL",
	    storageBucket: "YOUR_URL_STORAGE",
	    messagingSenderId: "YOUR_MESSAGING_KEY"
	  };
	  firebase.initializeApp(config);

7.- Correr el servidor:
	COMANDO: firebase serve

Listo :D


