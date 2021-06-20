# Deploy Laravel 8 en AWS (Menos de 5 minutos)


### Actualización de paquetes Ubuntu
`sudo apt-get update`  

`sudo apt-get upgrade`  

`sudo apt-get update`  

### Apache2
`sudo apt-get install apache2`  

### PHP 7.4
`sudo apt install php php-cli php-fpm php-json php-common php-mysql php-zip php-gd php-mbstring php-curl php-xml php-pear php-bcmath`  

### Composer
[https://getcomposer.org/download/](https://getcomposer.org/download/)  

### Modo reescritura Apache2
`sudo a2enmod rewrite`  


### Configuración Apache2 
`sudo nano /etc/apache2/apache2.conf`  

`<Directory /home/ubuntu/>
        Options Indexes FollowSymLinks
        AllowOverride All
        Require all granted
</Directory>
`  

###  Sitio por defecto Apache2  
`sudo nano /etc/apache2/sites-enabled/000-default.conf`  

### Configuración php.ini
`sudo nano /etc/php/7.4/apache2/php.ini`

### Reinicio del servidor Apache2
`sudo service apache2 restart`

### Instalación proyecto Laravel 8
`composer create-project laravel/laravel nombre_proyecto`  

### Video explicativo:
[https://youtu.be/uNjyopVYqHU](https://youtu.be/uNjyopVYqHU)


