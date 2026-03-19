# : Compresie și Decompresie : RLE-EASY

**Autor:** Glitter Geeks-Coderun 2025

Acest proiect implementează algoritmul **Run-Length Encoding (RLE)**.



## Mod de Folosire: 

Această aplicație rulează direct pe laptop, foarte simplu 


PAS 1:  toate fișierele (`index.html`, `style.css`, `app.js`, `README.md`) trebuie să fie puse în același folder.
PAS 2:  dublu-click pe fișierul **index.html** (astfel se va lansa aplicația)


##  DESPRE Interfață 

Aplicația are un singur câmp de intrare/ieșir și două butoane:

### 1. 𝐂𝐨𝐦𝐩𝐫𝐢𝐦𝐚

* **Rolul:** Aplică algoritmul **compressRLE()** pe conținutul din câmpul de text
    1.  Citește textul introdus ("AAACCCC")
    2.  Rulează funcția de compresie ("A3C4")
    3.  Afișează rezultatul codificat în același câmp de text


### 2. 𝐃𝐞𝐜𝐨𝐦𝐩𝐫𝐢𝐦𝐚

* **Rolul:** Aplică algoritmul invers, **decompressRLE()**, pe conținutul din câmpul de text

    1.  Citește textul **codificat** ("A3C4")
    2.  Rulează funcția de decompresie
    3.  Afișează textul original, complet în același câmp de text. ("AAACCCC")


## Principiul de Lucru (RLE)

RLE se bazează pe găsirea secvențelor de caractere identice și înlocuirea lor cu o pereche **[caracter][numarul de repetari]**

* **Compresie:** Dacă un caracter apare de n ori consecutiv, el este înlocuit cu [caracter][n]
		 Dacă n este 1, numărul este omis
    * *Exemplu:* **"AAAAA"** devine **"A5"**.
* **Decompresie:** 
		Se citește fiecare caracter, iar dacă el este urmat de cifre, repetă caracterul de numărul de ori specificat.

Co-authored-by: abcd <patricialeonte14@gmail.com>
