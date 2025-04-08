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
Des de webmin actualitza un paquet.
Utilitza webmin per instal·lar un joc de apt.
Utilitza webmin per instal·lar gimp de apt.
Utilitza webmin per desinatl·lar el joc que heu instal·lat abans.
4.- Serveis
Utilitza webmin per mostrar els serveis que s'inicien amb el sistema.
Utilitza webmin per mostrar els serveis que estan actius.
Utilitza webmin per mostrar l'estat del servidor Apache.
Utilitza webmin per aturar Apache.
Utilitza webmin per mostrar l'estat del servidor Apache apagat.
Utilitza webmin per reiniciar Apache.
Utilitza webmin per mostrar l'estat del servidor Apache reiniciat.
5.- Quotes de disc
Activa les quotes de disc pels usuaris amb la comanda:

sudo apt install quota quotatool
Utilitza webmin perquè l'usuari bakalao_X no pugui tenir més de 2 MB d'informació al disc.
Comprova que el límit de la quota funciona.
Utilitza webmin perquè l'usuari techno no pugui tenir més de 10 fitxers al disc.
Comprova que el límit de la quota funciona.
6.- Còpies de seguretat
Utilitzant el mòdul de Webmin Filesystem Backup fes una còpia de seguretat del directori /home al directori /backups (l'haureu de crear si no existeix).
Modifica alguns fitxers de /home.
Recupera la còpia de seguretat.
Comprova que els fitxers de /home són els correctes.
Programa una còpia de seguretat de /home/bakalao_X per els divendres a les 21:00.
Esborra la còpia de seguretat programada anteriorment.
7.- Compartició
Crea un recurs a webmin que, utilitzant samba, comparteixi una carpeta anomenada "area_public_X" per a usuaris sense autenticar en forma de lectura i escriptura.
Crea un recurs a webmin que, utilitzant samba, comparteixi una carpeta anomenada "pontaeri_privat_X" per a usuaris _X i techno només de lectura.
Comprovar des de Windows que aquests recursos funcionen.
