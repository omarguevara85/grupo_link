## Prueba
* Hora de inicio: 7:40 pm
* Hora de finalización: 10:40 pm
* El proyecto completo se encuentra en la carpeta _build junto a la copia de la base de datos
* Se realizo la exportacion de todas las configuraciones para un mejor despliegle en ambiente

> Nota: El proyecto no contempla estilos, ya que no se cuenta con un diseño previo aprobado, se realiza la creación del sub-theme y twig para posterior maquetación 

## Herramientas
* Drupal 9.3.3
* Composer
* Drush
* Git (develop - main)

## Proyecto

Realizar la implementación de un portal web de tipo One page para una empresa que ofrezca servicios de construcción de casas que tenga los siguientes componentes:
Secciones:
* Slideshow
* Proyectos
* Nosotros
* Contacto

## Instalación

Primero se debe [instalar composer](https://getcomposer.org/).

Segundo se debe ejecutar el comando `composer install` para que descargue todas las dependencias que se encuentran en el composer.json y que están ignoradas en el .gitignore

Tercero se instala mediante drush importando las configuraciones ya exportadas, aclarando que esta instalación no tendrá contenido.

```
vendor/drush/drush/drush site:install --config-dir=../config/sync --db-url=mysql://user:pass@localhost/name_bd --account-name=admin --account-pass=123456 --account-mail=omarguevara85@gmail.com --yes
```

Para sincronizar configuraciones de diferentes desarrolladores se debe tener en cuenta la ruta de exportación de configuración en el archivo settings.php

```
$settings["config_sync_directory"] = "../config/sync";
```
> Nota: El proyecto no contempla estilos, ya que no se cuenta con un diseño previo aprobado, se realiza la creación del sub-theme y twig para posterior maquetación 
