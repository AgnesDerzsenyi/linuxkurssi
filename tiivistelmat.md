# Raportin kirjoittaminen

-	Raportointi on työkalu, joka auttaa kirjoittajaa ja muita ymmärtämään kuvaamaansa prosessia.
-	Raportin on oltava toistettava, täsmällinen ja helppolukuinen.
-	Pienet yksityiskohdat voivat olla tärkeitä, kuten ympäristö, jossa prosessi suoritettiin, komennot ja niiden tulokset sekä niiden suorittamisajankohta.
-	Viitteiden käyttö on myös tärkeää, jotta raportti on akateemista tasoa
-	Raportin kirjoittaminen jostakin, jota ei ole tehty, on kirjoittajan ja lukijan ajanhukkaa ja siksi turhaa.
## Lähteet:
o	Karvinen, Tero: Raportin kirjoittaminen, 4.7.2006, luettavissa: Raportin kirjoittaminen | Tero Karvinen, luettu: 25.08.2023

# Mikä on Free Software?

-	Vapaa ohjelmisto tarkoittaa sitä, että käyttäjillä on vapaus käyttää, kopioida, jakaa, tutkia, muuttaa ja parantaa ohjelmistoa. Ohjelma on vapaa ohjelmisto, jos ohjelman käyttäjillä on nämä neljä olennaista vapautta.
-	"Vapaa ohjelmisto" ei tarkoita "ei-kaupallista". Päinvastoin vapaan ohjelman on oltava saatavilla kaupalliseen käyttöön, kaupalliseen kehittämiseen ja kaupalliseen jakeluun. Tämä politiikka on olennaisen tärkeä – ilman tätä vapaat ohjelmistot eivät voisi saavuttaa tavoitteitaan.
-	Vapaus käyttää ohjelmaa tarkoittaa minkä tahansa henkilön tai organisaation vapautta käyttää sitä missä tahansa tietokonejärjestelmässä, mihin tahansa yleiseen työhön ja tarkoitukseen ilman, että heidän tarvitsee kommunikoida siitä kehittäjän tai muun tietyn tahon kanssa. Tässä vapaudessa käyttäjän tarkoitus on tärkeä, ei kehittäjän tarkoitus.
-	Lähdekoodin saatavuus on välttämätön edellytys vapaalle ohjelmistoille. Lähdekoodi määritellään ohjelman suositeltavaksi muodoksi muutosten tekemiseen. Siten mikä tahansa muoto, jota kehittäjä muuttaa ohjelman kehittämiseksi, on kyseisen kehittäjän version lähdekoodi.
-	Jakeluvapaus tarkoittaa, että voit vapaasti jakaa kopioita, joko muuttamatta tai muuttamalla niitä, joko ilmaiseksi tai perimällä jakelumaksun, kenelle tahansa missä tahansa. Vapaus tehdä näitä asioita tarkoittaa (muun muassa), että sinun ei tarvitse pyytää tai maksaa lupaa tehdäksesi niin.
## Lähteet:
o	GNU Operating System: What is Free Software? Luettavissa: What is Free Software? - GNU Project - Free Software Foundation Luettu: 27.8.2023


# Raportti: Linux virtuaalikoneeseen

Tein harjoituksen sunnuntaina 2023-08-27 omalla tietokoneella. 
Koneena oli Lenovo IdeaPad S145-15IIL, käyttöjärjestelmä Windows 11 Home

1.	Avasin linkin: https://terokarvinen.com/2023/linux-palvelimet-2023-alkusyksy/#h1-virtuaali-linux ja valitsin linkin: https://terokarvinen.com/2021/install-debian-on -virtualbox/?fromSearch=virtualbox nähdäksesi ohjeet Debianin asentamisesta Virtualboxiin.
16:03
2.	Latasin Debianin ISO-otoksen aiemmin, joten tarkistin, onko minulla kuvauksessa oleva versio.
16:06
3.	Latasin aiemmin VirtualBoxin ja se on asennettu tietokoneelleni. Latauslinkki on kuvauksessa ja ladattu tiedosto on .exe-tiedosto, joten kaksoisnapsauttamalla sitä käynnistyy asennus.
16:09
4.	Käynnistin VirtualBoxin Windowsissa ja valitsin Machine -> New
16:13
5.	Ensimmäisessä avautuvassa ikkunassa oli valittava Expert-tila. virtuaalikoneen piti antaa:
•	-nimi: virtuaalikone
•	-tyyppi: Linux
•	-versio: Debian (64-bittinen)
•	"Ohita valvomaton asennus" on valittava
16:24
6.	Hardware-valikossa Memory on suositeltavaa asettaa arvoon 4000 MB
16:26
7.	Prosessorin asetukset jätin ennalleen
8.	Hard disk: Valitsin: Luo virtuaalinen kiintolevy nyt – kyllä.
9.	Napsautin "Finish"
16:31
10.	Näin uuden virtuaalikoneen vasemmalla VirtualBox Managerissa.
16:32
11.	Etsin Create Virtual Hard Disc -ikkunaa noin 10 minuuttia, enkä ollut varma, loinko virtuaalikoneen oikein.
16:43
12.	Jatkoin ohjeiden noudattamista, seuraava vaihe on:
Insert Debian ISO Image as a Virtual CDROM
16:45
13.	Valitsin luomani virtuaalikoneen ja valitsin:
Settings->Storage
16:48
14.	"Controller IDE" -kohdan ohjeiden mukaan minun pitäisi nähdä CDROM tyhjä, mutta näytölläni se on bedian-live-121.0... luultavasti siksi, että valitsin tiedoston asennuksen aikana. Kokeilen toimiiko virtuaalikone tällä tavalla vai täytyykö minun aloittaa prosessi uudelleen.
16:52
15.	Käynnistin virtuaalikoneeni kaksoisnapsauttamalla sitä VirtualBox-valikossa
16:54
16.	live-työpöytä ilmestyi
17:00
17.	Testasin työpöytää valitsemalla vasemmasta yläkulmasta "Sovellukset"-valikosta "Web-selain". Googlasin "Tero Karvinen", klikkasin ylälinkkiä ja näin kotisivun. Sitten suljin selaimen.
17:03
18.	Suoritan Debianin asennusohjelman kaksoisnapsauttamalla "Install Debian" -kuvaketta vasemmassa reunassa
17:05
19.	On "Debian GNU/Linux Installer" (Calamares)
o	Welcome: Language: American English 
o	Location: Finland (clicked it on the map)
o	Keyboard. I choose the keyboard you have.
o	Partitions: -> Erase disk: yes 
o	Users 
- "What is your name?": Agnes Derzsenyi
- "What name do you want to use to log in?" agnes
- "What is the name of this computer?" virtualmachine 
- "Choose password to keep your account safe."
- "Log in automatically without asking for the password" No.
o	Summary
o	Backups 
o	Click "Install".
17:16
20.	"All done." "Restart now" - Yes. Click "Done."
17:29
21.	Kirjauduin sisään käyttäjätunnuksellani ja salasanallani
17:32
22.	Avasin terminaalin: Sovellukset: Terminal Emulator
17:45
23.	Kirjoitin: ”sudo apt-get update” ja annoin salasanani
17:47
24.	Kirjoitin "sudo apt-get -y dist-upgrade"
17:49
25.	Valmis 17:55
26.	Kirjoitin "sudo apt-get -y install ufw" asentaakseni palomuurin
17:56
27.	Otin palomuurin käyttöön kirjoittamalla "sudo ufw enable"
17:57
28.	Käynnistin järjestelmän uudelleen valitsemalla vasemmasta yläkulmasta "Sovellukset"-valikosta: Kirjaudu ulos: Käynnistä uudelleen

Parempaa resoluutiota varten asensin "VirtualBox Guest Addition"
1.	Kirjauduin virtuaalikoneeseeni ja "Devices"-valikosta valitsin "Insert Guest Additions CD image"
18:03
2.	Menin kohtaan Sovellukset -> Tiedostonhallinta -> "VBox_GAs.."
18:05
3.	Avasin Terminal Emulatorin ja vaihdaakseni hakemistoa, kirjoitin: 
$ cd /media/*/VBox*
$ ls (ilman $ merkkiä)
4.	Suoritin asennusohjelma kirjoittamalla ” sudo bash VBoxLinuxAdditions.run”
18:07
5.	Valmista tuli 18:09
6.	Käynnistin järjestelmän uudelleen kohdasta Sovellukset ->Kirjaudu ulos -> Käynnistä uudelleen
7.	Resoluutio kasvoi uudelleen sisäänkirjautumisen jälkeen, joten tallensin edistymisen valitsemalla "Machine-> Take snapshot"
18:14


