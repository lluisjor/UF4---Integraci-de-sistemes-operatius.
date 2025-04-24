# Administració de servidors amb Webmin
![image](https://github.com/user-attachments/assets/afe29797-c334-45ed-ac85-ff6d2ede782b)

## 👤 Nom de l’alumne: Pit i Marc

# 📑 Índex

Creació i modificació d’usuaris

Programació de tasques

Instal·lació de software

Serveis

Quotes de disc

Còpies de seguretat

Compartició amb Samba



## EJERCICIOS


## 1.- Crear i modificar usuaris
Fer tot des de webmin

Has de crear dos usuaris bakalao_X i techno_X on (X és el vostre cognom).


Els usuaris et passaran el hash de la seva contrasenya, no la contrasenya real. (podeu fer servir openssl).

![image](https://github.com/user-attachments/assets/107b4b09-f485-4099-8802-63da92b611f8)

Cada usuari tindrà un directori a home igual al seu nom d'usuari.
Utilitzaran bash com a shell.
Els usuaris estaran dins del grup que tingui el seu mateix nom i dins del grup usuaris_empresa.

![image](https://github.com/user-attachments/assets/cca675c5-f593-4b20-b7d8-8e1da09bee01)

L'usuari techno no podrà fer login després del dia 31-03-2025.

![image](https://github.com/user-attachments/assets/d4449a95-2594-46fc-a4a2-7ef0641c412c)

Comproveu que els usuaris poden iniciar sessió.
Canvia la data del sistema (utilitzant webmin) i comprova que techno no pot iniciar sessió si estem a dia 01-04-2025.

![image](https://github.com/user-attachments/assets/c59d4ecb-6d86-4be8-abf1-afedd144f72b)


### 2.- Programar tasques

Programa una tasca que neteja els paquets de Linux que ja no s'utilitzen una vegada al mes.

![image](https://github.com/user-attachments/assets/b814bce8-6dcd-4452-ba59-2f28109075b2)


Programa una tasca diaria que apaga l'ordinador a les 14:00.

![image](https://github.com/user-attachments/assets/2cbc788d-f060-4937-b111-a61d274b66d1)


Comprova que funcionen (canvia dia i hora del sistema mitjançant webmin).


3.- Instal·lació de software
Utilitza webmin per mostrar quins paquets de software es podrien actualitzar.

![Captura desde 2025-04-22 11-01-39](https://github.com/user-attachments/assets/e770f661-12e9-4a11-b3b1-e5fdeccd670e)

Des de webmin actualitza un paquet.

Utilitza webmin per instal·lar un joc de apt.

![Captura desde 2025-04-22 11-13-07](https://github.com/user-attachments/assets/c990503f-0bf9-41c9-ada2-3e2133e0f7cb)


Utilitza webmin per instal·lar gimp de apt.

![Captura desde 2025-04-22 11-17-32](https://github.com/user-attachments/assets/4abded03-6b09-46a5-82cd-3dd830cfb1d5)


Utilitza webmin per desinatl·lar el joc que heu instal·lat abans.

![Captura desde 2025-04-22 11-19-26](https://github.com/user-attachments/assets/6f0f7746-36fe-43b4-8884-2f21484f20e1)


4.- Serveis
Utilitza webmin per mostrar els serveis que s'inicien amb el sistema.
Utilitza webmin per mostrar els serveis que estan actius.

![Captura desde 2025-04-22 11-24-24](https://github.com/user-attachments/assets/4d05a0ab-098c-4d97-852e-2192f4fbca44)


Utilitza webmin per mostrar l'estat del servidor Apache.

![Captura desde 2025-04-22 11-24-24](https://github.com/user-attachments/assets/7c8bc7b2-d08a-47cd-8d9f-3908faf69412)


Utilitza webmin per aturar Apache.

![Captura desde 2025-04-22 11-29-50](https://github.com/user-attachments/assets/81f01584-4d04-47a0-8a83-13e5e9a19f1a)


Utilitza webmin per mostrar l'estat del servidor Apache apagat.
Utilitza webmin per reiniciar Apache.
Utilitza webmin per mostrar l'estat del servidor Apache reiniciat.




5.- Quotes de disc
Activa les quotes de disc pels usuaris amb la comanda:

sudo apt install quota quotatool

![Captura desde 2025-04-22 11-33-49](https://github.com/user-attachments/assets/3c0daa42-c8d0-4c83-bcd2-3f82a69bc369)


Utilitza webmin perquè l'usuari bakalao_X no pugui tenir més de 2 MB d'informació al disc.

![Captura desde 2025-04-22 11-43-10](https://github.com/user-attachments/assets/771d6418-7ff1-49e8-b294-2156b2672796)


Comprova que el límit de la quota funciona.
Utilitza webmin perquè l'usuari techno no pugui tenir més de 10 fitxers al disc.



![Captura desde 2025-04-22 12-11-03](https://github.com/user-attachments/assets/41fbcb57-9d3e-4f35-9b46-537329270f1a)


Comprova que el límit de la quota funciona.


![Captura desde 2025-04-22 12-19-38](https://github.com/user-attachments/assets/465ae78f-f7ce-4e77-b065-ae7a959fff02)


6.- Còpies de seguretat
Utilitzant el mòdul de Webmin Filesystem Backup fes una còpia de seguretat del directori /home al directori /backups (l'haureu de crear si no existeix).


![Captura desde 2025-04-22 12-29-12](https://github.com/user-attachments/assets/1f136c3b-5106-4e36-b142-ca696bbf21a5)


Modifica alguns fitxers de /home.
Recupera la còpia de seguretat.
Comprova que els fitxers de /home són els correctes.
Programa una còpia de seguretat de /home/bakalao_X per els divendres a les 21:00.


![Captura desde 2025-04-22 12-19-38](https://github.com/user-attachments/assets/ce7640ad-ff40-445f-85c3-b937964708ce)


Esborra la còpia de seguretat programada anteriorment.

![Captura desde 2025-04-22 12-32-43](https://github.com/user-attachments/assets/8c5eb608-3d63-4fda-ae16-91b1daed6619)


7.- Compartició
Crea un recurs a webmin que, utilitzant samba, comparteixi una carpeta anomenada "area_public_X" per a usuaris sense autenticar en forma de lectura i escriptura.
Crea un recurs a webmin que, utilitzant samba, comparteixi una carpeta anomenada "pontaeri_privat_X" per a usuaris _X i techno només de lectura.
Comprovar des de Windows que aquests recursos funcionen.
