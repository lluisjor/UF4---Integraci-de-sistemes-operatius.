# Actividad 1 - Compartir una impresora de Linux en Windows

Su oficina dispone de una impresora centralizada que está conectada a un equipo con Linux. El resto de ordenadores de la oficina utilizan Windows 10. Has de fer que todos los usuarios pueden utilizar la impresora. La xarxa de l'oficina fa servir aquestes adreces IP. On X es el número asignado al grupo.

![324541555-744d6524-d1c8-4edd-9a9a-fba6acf0a776](https://github.com/user-attachments/assets/aafd8c7f-c9a2-4721-b7ca-236923b575ee)


Instalaremos los CUPS con los siguientes comandos: 
- sudo apt update
- sudo apt install cups

Luego instalaremos la impresora PDF virtual con este comando
sudo apt install printer-driver-cups-pdf

Luego abriremos el navegador y buscaremos lo siguiente: http://localhost:631
Nos llevara a la siguiente pagina.

![415101396-74db4eb0-cd4c-4a49-9527-16202cf53a1f](https://github.com/user-attachments/assets/c84edcb7-bec1-4174-ae39-c628ce9e19c9)

Le daremos a Administracion y luego donde pone "Añadir impresora"
![415102779-2c978f01-79f4-4da2-ba2c-8855ab110cab](https://github.com/user-attachments/assets/0a419881-7dd2-403f-9339-d99ceb0bd2b6)

Y seguiremos estos pasos:
1r

![415106734-f384bccf-face-4654-9852-0d862f2c58ef](https://github.com/user-attachments/assets/52e3acda-f683-4903-8ce0-55da7796af59)

2n

![415107091-02eb9b25-59d5-4d3a-ba44-308dc0f12795](https://github.com/user-attachments/assets/c2283118-212a-4a05-a7dc-63e9a1b419e8)

3r

![415107858-d162713f-04fa-4941-aaae-50ea41d520d0](https://github.com/user-attachments/assets/974ddedd-5652-4356-ad01-932430099d32)

4t

![415108018-5356d665-b06c-4260-b1ba-4a9f49e102f9](https://github.com/user-attachments/assets/8c6c1049-c40f-44db-8490-28f72579e1d6)

Y finalmente le daremos a Añadir impresora.

Lo siguiente dentro del terminal, deberemos cambiar la siguiente configuración dentro de este documento: /etc/cups/cupsd.conf

![Captura de pantalla 2025-04-09 235340](https://github.com/user-attachments/assets/c1175781-4422-46c2-9e71-312176cb7b13)




Luego reiniciaremos el servicio de CUPS
sudo systemctl restart cups

Finalmente iremos a Windows para poder acceder a la impresora que hemos compartido de Linux.

Hay muchas maneras pero hemos elegido la siguiente.

En el buscador de Windows, buscaremos impresoras y escaners.

LuegoLe daremos a Agregar  impresoras o escaners.

![Captura de pantalla 2025-04-09 235037](https://github.com/user-attachments/assets/135f77ff-e405-4de3-ada7-85dbf28bb7c2)

Le daremos a la 3r opcion.

![Captura de pantalla 2025-04-09 235546](https://github.com/user-attachments/assets/d8bce94d-443c-4e72-82a0-88892962cb2c)

Luego A dispositivo TCP/IP y rellenaremos.

![Captura de pantalla 2025-04-09 235647](https://github.com/user-attachments/assets/ef8f9bfa-1729-476f-8507-2f1fcb99a66a)

Y al final ya la tendremos con el nombre que queramos.

![Captura de pantalla 2025-04-09 235918](https://github.com/user-attachments/assets/22cac0fd-db63-474c-ad53-a46f80b5a9bb)


# Actividad 2 - Compartir una impresora de Windows a Linux

Su oficina dispone de una impresora centralizada que está conectada a un equipo con Windows 10. El resto de ordenadores de la oficina utilizan Linux. Has de fer que todos los usuarios puguin utilicen la impresora. La xarxa de l'oficina fa servir aquestes adreces IP. On X es el número asignado al grupo.

![324541597-1dd6f371-1038-4f82-82cc-35fe39793671](https://github.com/user-attachments/assets/082c22f0-a80b-4bed-9b15-3a87bcb35849)


Descargamos en programa PDFCreator para la tener una la impresora 
![image](https://github.com/user-attachments/assets/a5e08a99-c006-4064-84bb-27f112724d6f)

Buscamos Paenl de control y entramos


![image](https://github.com/user-attachments/assets/f6f50a19-0f01-4641-952a-452b7ebe7d5b)

Ahora buscamos dispositius i impressores
![image](https://github.com/user-attachments/assets/8a67b088-939a-4dc7-b915-cb6108a89dc3)

Cuando entramos ahi nos salen los dispositivo y las impresoras y ahi nos saldra la que hemos instalado  PDFCreator todo esto demomento en win10

![image](https://github.com/user-attachments/assets/0017cb05-6dcf-4b1d-add0-46912bd85ffe)

Ahora vamos a Ubuntu

Ponemos esta comanda que para poner una impresora
![image](https://github.com/user-attachments/assets/f86e70b6-ba49-4068-b505-2930aa66b09f)


Le damos a añadir, le damos a impresora de xarxa (Impressora windows a traves de samba) 
![image](https://github.com/user-attachments/assets/be1b8465-0f34-48b4-9be9-fd56e1158093)

Aqui ponemos la ip de la maquina de windows y el nombre, tambien ponemos la contraseña y el nom de usuari, cuando este la tendras que configurar pero me he olvidado las capturas.
![image](https://github.com/user-attachments/assets/4bda1906-0951-4615-8023-b77a56ef289e)

y como vemos aqui esta la impresora 


![image](https://github.com/user-attachments/assets/68684a1c-b7ad-4a73-949e-769cfaca58de)




 ahora le damos a la impresora y imprimimos 
 
 Y AQUE VEMOS QUE SE ESTA IMPRIMIENDO :)

 ![image](https://github.com/user-attachments/assets/f85e359c-761f-4cd2-ba10-c123f23e9a78)

![image](https://github.com/user-attachments/assets/f0c3b4d2-efc5-4b72-8ffa-75fb68ab4af5)
