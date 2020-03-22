Instalación
1 Clone este repositorio
   https://github.com/Tomiello/Live-Chat
   
2 Instalar paquetes con composer
    cd laravel-chat
    $ composer install
    
3 Crear y configurar un archivo .env
    hacer una copia de .env.example y renombrarla como .env
    $ php artisan key:generate
    poner credenciales de base de datos en el archivo .env 
    
4  Correr las migraciones 
     $ php artisan migrate
     
5 Crear y configurar una cuenta de pusher
    ingresar en https://pusher.com/ y crear una nueva app
    poner credenciales de empujador al archivo .env 
    remplace PUSHER_APP_KEY en su app.blade.php

   var pusher = new Pusher('aca va la clave', {
      cluster: 'ap2',
      forceTLS: true
   });
