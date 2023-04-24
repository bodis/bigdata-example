# Bigdata pelda projekt
A feladat a következő:
1. adott a ```dataset/small``` könyvtárban 2 CSV fájl (ezek a rendes Rottentomato adatfájlokból lettek kivágva körülbelül)
2. a CSV fájloknak van fejléce, de nekünk igaziból csak a következők lesznek fontosak
    * ```rotten_tomatoes_movies.csv``` fájlból az ```id, title, runtimeMinutes, releaseDateTheaters``` oszlopok
    * ```rotten_tomatoes_movies_reviews.csv``` fájlból az ```id, creationDate, originalScore``` oszlopok
    * a review CSV-ben az ID mezők egyezik meg a movies CSV ID mezőjével
3. pár egyszerű összegzést / lekérdezést kellene csinálni a fenti CSV-kből (a lekérdezés leírásait lásd lentebb) 
4. maga az eredmény is lényeges de a cél az lesz hogy ekkora adatkört ismerve kellene írni olyan kódot ami szerintetek hatékonyan fog futni az ennél jóval nagyobb adatmennyiségen is (sajnos a teljes adatmennyiség sem lesz azért annyira óriási; 143.258db film, kb. 1.5m review)
5. a teljes CSV-k nem kerülhetnek fel ide mert 100MB-os a max fájl méret ami itt engedélyezve van.
6. mire figyelj: memória limit? CPU meddig fut? tudod párhuzamosítani? mennyire egyszerű a kód?
7. mire ne figyelj: mindegy milyen nyelvben kódolsz

# FAQ
* CSV értékelés mezőjét hogy kell értelmezni?
   * amiben sima 0-5 szám van az maga az értékelés (5-ös skálán)
   * amiben csak betűk vannak vagy üres az skip
   * amiben X / Y a formátumban szerepelnek számok (space-k nem számítanak) azt arányosítani kell 5-ös skálára (a legtöbb így van)

# Feladat 1
Az átlag legjobb értékelést kapott TOP 3 film.

# Feladat 2
Évekre bontott adatok alapján a legjobb átlagos értékeléseket kapott TOP 3 film+év páros. Tehát lehet lepontoztak egyik évben egy filmet, de a másik évben meg jól felpontozták akkor a filmhez a legjobb ilyen év számít és ezekből számolunk TOP 3-at.

# Feladat 3
Melyik években voltak a legrosszabb értékelésűek a filmek (TOP 3).

# Feladat 4
A filmek hossza alapján 10 perces bontásokban milyen átlagos értékeléseket kaptak a filmek (csoportok, 0-9, 10-19, ..., 80-89, ...)

# Feladat 5
Az egyes filmek kiadási dátumához képest mi a legnagyobb távolságban létező review érték.






