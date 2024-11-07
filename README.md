# BAlexM_SzuperhosPojekt

1. Hozz létre egy új projektet SzuperhosProjekt néven. A projektet az alábbi template 
repo alapján készítsd: 
https://github.com/darkbeast0106/Java-SzuperhosProjekt-template 
a. GitHub-on bejelentkezés után a ’Use this template’ gombra kattintva hozz létre 
új GitHub repot, melynek nevét „SajatNev_SzuperhosProjekt” formában add 
meg. Az így létrehozott repot klónozd le és abban dolgozz. 
b. A main modulban található hu.petrik.szuperhosprojekt packageben dolgozz. 
A további osztályokat ebben a packageben hozd létre. A test modulban ne 
végezz módosítást. 
c. Ügyelj rá, hogy a feladat megoldása során ékezetmentes azonosítókat 
használj. Az elkészült projektben ne maradjon szintaktikai hiba, még a 
tesztesetekben sem. 
d. A tesztesetekben használt osztályok, metódusok még nem léteznek így hibára 
fog futni az egész projekt. Ennek elkerüléséhez, generálj le minden függvényt, 
vagy az alábbi megoldást használd: https://stackoverflow.com/a/16784855 
e. Ha a futtatás során nem megfelelően jelennek meg az ékezetes karakterek 
akkor az alábbi beállítást hajtsd végre IntelliJ-ben: 
i. menüsoron: 
Help 
Edit Custom VM Options... 
ii. A megnyitott fájl végére az alábbi sort írd be: -Dfile.encoding=UTF-8 
iii. Indítsd újra az IntelliJ-t 
2. Írj egy Szuperhos interfészt, ami egy legyoziE metódust tartalmaz. A metódus 
paramétere egy Szuperhos, és egy logikai értékkel tér vissza. Legyen egy 
mekkoraAzEreje metódusa is, ami nem kér paramétert, és a Szuperhos erejét fogja 
visszaadni.  
3. Írj Milliardos interfészt, ami egy visszatérés nélküli kutyutKeszit() metódust tartalmaz  
4. Írj egy Bosszuallo absztrakt osztályt, ami implementálja a Szuperhos interfészt.  
▪ Az osztály a következő private láthatóságú adattagokkal rendelkezik: egy 
lebegőpontos szuperero, és egy logikai vanEGyengesege.  
▪ Az osztály rendelkezzen paraméteres konstruktorral, ami beállítja az 
adattagokat.   
▪ Legyen egy public megmentiAVilagot absztrakt metódusa, ami egy logikai 
értékkel tér vissza. Valósítsd meg továbbá az interfész metódusait. Az erő 
lekérdezésekor add vissza a Bosszuallo szupererejét. Egy Bosszuallo egy 
Bosszuallo szuperhőst akkor tud legyőzni, ha annak van gyengesége, és ereje 
kisebb, mint az övé. Batman-t csak akkor tudja legyőzni, ha ereje kétszer nagyobb.  
▪ Az osztálynak legyen továbbá getter és setter metódusa az adattagjaihoz, és 
legyen szöveges formára alakítható, kiírva az adattagok értékét, pl.: 
▪ Szupererő: 120,21; van gyengesége 
▪ Szupererő: 30; nincs gyengesége 
▪ Ügyelj rá, hogy a kiíratás során csak a szükséges mennyiségű tizedesjegyeket 
írd ki, ehhez használd a java.text.MessageFormat osztály format() metódusát. 
példa a használathoz: https://igorstechnoclub.com/string-formatting-in-java
with-messageformat/ 
Oldal 1 
Interfacek – Szuperhős 
5. Írj egy Vasember osztályt, ami a Bosszuallo leszármazottja, és megvalósítja a 
Milliardos interfészt.  
▪ Az osztálynak egy default konstruktora legyen, ami beállítja a Vasember 
tulajdonságait. A Vasember szuperereje 150, és van gyengesége.  
▪ Ha a Vasember kütyüt készít, akkor szuperereje nőjön ereje egy 0-10 közötti 
véletlenszerű lebegőpontos számmal.  
▪ A Vasember akkor menti meg a világot, ha a szuperereje nagyobb, mint 1000.  
▪ Az osztály legyen továbbá szöveges formára alakítható. Az adattagok értékein 
kívül írja ki azt is, hogy a Vasemberről van szó.  
6. Írj egy Batman osztályt, ami implementálja a Szuperhos és Milliardos interfészeket.  
▪ Az osztálynak legyen egy lebegőpontos lelemenyesseg adattagja.  
▪ Az osztály rendelkezzen egy default konstruktorral, ami 100-ra állítja az 
adattag értékét. A metódusai az alábbiak szerint legyenek megvalósítva: Batman 
ereje a leleményességének kétszeresével egyezik meg, és bármilyen Szuperhőst 
képes legyőzni, akinek ereje kisebb, mint Batman leleményessége. Ha Batman 
kütyüt készít, akkor a leleményessége 50-el nő.  
▪ Az osztály legyen szöveges formára alakítható, ami kiírja, hogy Batmanről van 
szó, és megadja a leleményességét. Itt is figyelj a tizedesjegyek számára, pl.: 
▪ Batman: leleményesség: 400 
7. Írj egy Kepregeny nevű futtatható osztályt. Az osztály rendelkezzen egy szereplok 
statikus függvénnyel, ami egy fájl elérési útját várja paraméterül, visszatérése pedig 
void. A metódus feladata, hogy a fájlból beolvasott sorokat feldolgozza, és 
létrehozzon belőlük Batman, vagy Vasember objektumpéldányokat, majd ezekre 
meghívja a kutyutKeszit metódust annyiszor, ahányszor az aktuális sor írja. Ezeket 
egy publikus statikus listában tárold le az osztályban, a lista neve szuperhosLista 
legyen. 
8. Készíts továbbá egy szuperhosok statikus metódust, ami végigmegy a tárolóban tárolt 
szuperhősökön, és kiírja őket.   
9. Hívd meg a main függvényben sorban a fenti két metódust. Minden esetleges kivételt 
(főleg: IOException) kezelj le vagy kivétel specifikációval, vagy try blokkban!  
Egy minta fájl felépítése az alábbi:  
Vasember 5 
Batman 8
