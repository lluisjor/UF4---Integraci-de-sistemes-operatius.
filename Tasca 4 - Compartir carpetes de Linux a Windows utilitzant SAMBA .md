Activitat 1

Crea una carpeta a la MV Linux a /srv/samba/compartida1 amb els permisos necessaris perquè pugui accedir tothom.

![image](https://github.com/user-attachments/assets/2714ce98-b8bc-4988-8da8-fb91aa8af911)


Crea la configuració de SAMBA per compartir la carpeta per a convidats (sense autenticació) amb lectura i escriptura.

![image](https://github.com/user-attachments/assets/9856e0fb-a332-4fa2-82b2-abb0cd6dfda9)

![image](https://github.com/user-attachments/assets/44611727-2c2c-4955-9e4c-2e807b4785ec)

![image](https://github.com/user-attachments/assets/ec0a0b27-53a3-4d7b-9bd2-b6f23bf50188)


Reinicia el servei SAMBA.

![image](https://github.com/user-attachments/assets/3c674879-3f83-4aa4-a92c-c92309e19078)

Comprova que tens accés des de Windows.

![image](https://github.com/user-attachments/assets/fb3d33d0-170e-456e-ae02-bc9ebf913c86)


Crea algun fitxer a la carpeta.

![image](https://github.com/user-attachments/assets/1441e887-3118-470b-adff-910e1a2ddf60)


Comprova que s'ha creat a Linux.

![image](https://github.com/user-attachments/assets/e6be79e5-501a-4787-9784-26c70018a40f)


Activitat 2

Crea una carpeta a la MV Linux a /srv/samba/compartida2 amb els permisos necessaris.

![image](https://github.com/user-attachments/assets/6922c92e-b191-4700-8dcf-6e00b1504ae9)


Crea un usuari local anomenat user1_X (on X és el teu cognom).

![image](https://github.com/user-attachments/assets/fed5030b-358f-4f0f-be0d-d956326c42a9)


Afegeux l'usuari anterior a SAMBA.

![image](https://github.com/user-attachments/assets/37df10e7-a237-45eb-8321-408923b0869b)


Crea la configuració de SAMBA per compartir la carpeta per a l'usuari anterior amb lectura i escriptura amb màscara
de fitxers 755.

![image](https://github.com/user-attachments/assets/77daa3a6-4d49-438d-bbee-13afdfb3f2ed)



Reinicia el servei SAMBA.

![image](https://github.com/user-attachments/assets/4270bc76-8517-4d03-b97b-1936754f16f2)


Comprova que tens accés des de Windows amb les credencials de l'usuari.
Crea algun fitxer a la carpeta.

![image](https://github.com/user-attachments/assets/09ded427-9e8f-446e-906a-31568032dcc1)

Comprova que s'ha creat a Linux i té els permisos 755.


![image](https://github.com/user-attachments/assets/7840d92e-84c7-4ac4-910d-d3cf38a0ac15)
