# COM INSTAL·LAR OWNCLOUD PER COMANDES


Primera comanda sira per instal·lar l'apache

![alt text](apache2.png)

## Instal·lar MariaDB
Una vegada tenim instal·lat el apache instal·larem la base de dades MariDB

![alt text](comanda3.png)

Seguidament posarem aquesta comanda

![alt text](ara.png)

Ara rainiciarem la base de dades per generar els canvis

![alt text](comanda5.png)

Ara posem esta comanda que ens permet tenir tots els permisos

![alt text](curios.png)

I podrem entrar a la linea de comandes de MariaDB


## Instal·lació PHP

Instalarem el software necessari

![alt text](seguent.png)


Primer instal·larem els repositoris

![alt text](php.png)


Ara si que ja podrem instalar PHP amb la versió corresponent

![alt text](phpya.png)

Ara tindrem que editar el PHP per aixo posarem lacomanda nano

![alt text](phpedit.png)

Lo que tindrem que editar es =

* File_uploads
* On allow_url_fopen
* On memory_limit = 256M upload_max_filesize
* 100M display_errors = Off
* Date.timezone = Europe/Madrid

Quan ja ho tindrem editat ctrl+o per guardar i cntrl+x per sortir
 
## Intal·lació Owncloud

![alt text](owncloud2.png)

Ara mourem a la carpeta corresponent

![alt text](owncloud3.png)

Seguidament cambiarem el propietari del arxiu

![alt text](cambiar.png)

També li cambiarem els permisos

![alt text](permisos.png)

També editarem aquest archiu i tindrem que copiar aquest text

![alt text](pablo.png)

![alt text](copiar.png)

Finalment posarem aquestes 6 comandes:

* sudo a2ensite owncloud.conf
* sudo a2enmod rewrite

* sudo a2enmod headers
* sudo a2enmod env
* sudo a2enmod dir
* sudo a2enmod mime

Ara tindrem que reiniciar l'apache 

**Ara ja podrem accedir al owncloud posarem la nostra IP /owncloud**

![alt text](anuel.png)

Procedirem a cambiar el domini per lo tant tindrem que entrar a aquesta ruta:

![alt text](owncloud1.png)

Una vegada al directori posarem la comanda sudo nano owncloud.conf i tindrem que copiar el text del principi cambiant el nom del servidor.

![alt text](owncloud2.png)


![alt text](owncloud3.png)

Posarem aquesta comanda


![alt text](owncloud4.png)

I per ultim reiniciarem l'apache


![alt text](owncloud5.png)

Ens sortira aixó

![alt text](owncloud6.png)

Ara per a que no ens surtigue correcte tindre que editar un fitxer.

Accedirem  aquest fitxer i editarem la IP posarem la del nostre servidor

![alt text](owncloud7.png)

Posarem el nom nou del domini i ja podrem accedir

![alt text](owncloud9.png)

Aquí o podem comprobar.

![alt text](owncloud11.png)
