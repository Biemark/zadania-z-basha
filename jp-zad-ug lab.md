## Bash -- zadania

1\. Używając linii poleceń stwórz struktur## Bash -- zadania

1\. Używając linii poleceń stwórz strukturę katalogów:

```sh
mkdir temp/{dom,nauka/{c,logo,pascal},praca/{dokumenty,zlecenia/{zrealizowane,niezrealizowane}}} -p
```

2\.Przejdź do katalogu dom i utwórz katalog wazne-sprawy.

```sh
cd dom
mkdir wazne-sprawy
```

3\Wejdź do katalogu wazne-sprawy i utwórz tam pusty plik rachunki.txt.

```sh
cd wazne-sprawy
touch rachunki.txt
```

4\.Będąc w katalogu wazne-sprawy skopiuj plik rachunki.txt do katalogu zrealizowane.

```sh
cp rachunki.txt ~/temp/praca/zlecenia/zrealizowane/
```

5\.Przejdź do katalogu zrealizowane i zmień nazwę pliku rachunki.txt na wykonano.txt.

```sh
cd ~/temp/praca/zlecenia/zrealizowane/
mv rachunki.txt wykonano.txt
```

6\.Utwórz plik wykonano.txt wielkości 11 bajtów, następnie podziel go pliki wielkości 5 bajtów. W ten sposób otrzymasz 3 pliki.

```sh
touch wykonano.txt
atom wykonano. txt
```
_Okazuje się, że gdy wpiszemy w plik .txt ciąg znaków '1234567890' to plik ten ma  11 bajtów. ;)_

```sh
split -b 5 wykonano.txt
```
7\.Będąc w katalogu logo skopiuj powyżej otrzymane 3 pliki do katalogu dokumenty.

```sh
cd ~/temp/nauka/logo/
cp ~/temp/praca/zlecenia/zrealizowane/{xaa,xab,xac} ~/temp/praca/dokumenty/
```
8\.Będąc w katalogu dokumenty połącz skopiowane 3 pliki w plik odtworzono.txt, tak aby otrzymać plik o zawartości identycznej z wykonano.txt. Następnie plik odtworzono.txt skopiuj do katalogu wazne-sprawy.

```sh
cat xaa xab xac > odtworzono.txt
cp odtworzono.txt ~/temp/dom/wazne-sprawy/
```
9.\Będąc w katalogu wazne-sprawy sprawdź, czy są jakieś różnice w zawartości plików wykonano.txt i odtworzono.txt.

```sh
_Brak jakichkolwiek różnic. :)_
```

10.\Wyświetl kalendarz na październik 2009 r.

```sh
cal oct 2009
```


Wyświetl kalendarz na wrzesień, październik i listopad 2009 r. z miesiącami obok siebie (cal):

    wrzesień 2009       październik 2009        listopad 2009  
ni po wt śr cz pi so  ni po wt śr cz pi so  ni po wt śr cz pi so  
       1  2  3  4  5               1  2  3   1  2  3  4  5  6  7  
 6  7  8  9 10 11 12   4  5  6  7  8  9 10   8  9 10 11 12 13 14  
...                   ...                   ...

```sh
cal -3 oct  20
```

Wyświetl kalendarz na październik, listopad i grudzień 2009 r. w taki sposób:

     październik             listopad               grudzień  
ni po wt śr cz pi so   ni po wt śr cz pi so   ni po wt śr cz pi so  
             1  2  3    1  2  3  4  5  6  7          1  2  3  4  5  
 4  5  6  7  8  9 10    8  9 10 11 12 13 14    6  7  8  9 10 11 12  
11 12 13 14 15 16 17   15 16 17 18 19 20 21   13 14 15 16 17 18 19  
...                    ...                    ...  

```sh
cal -3 nov 2009
```
I jeszcze raz na wrzesień i październik oraz na październik i listopad 2009 r z miesiącami obok siebie:

     październik             listopad  
ni po wt śr cz pi so   ni po wt śr cz pi so  
             1  2  3    1  2  3  4  5  6  7  
 4  5  6  7  8  9 10    8  9 10 11 12 13 14  
11 12 13 14 15 16 17   15 16 17 18 19 20 21  
...                    ...







ę katalogów:

```sh
mkdir temp/{dom,nauka/{c,logo,pascal},praca/{dokumenty,zlecenia/{zrealizowane,niezrealizowane}}} -p
```

2\.Przejdź do katalogu dom i utwórz katalog wazne-sprawy.

```sh
cd dom
mkdir wazne-sprawy
```

3\Wejdź do katalogu wazne-sprawy i utwórz tam pusty plik rachunki.txt.

```sh
cd wazne-sprawy
touch rachunki.txt
```

4\.Będąc w katalogu wazne-sprawy skopiuj plik rachunki.txt do katalogu zrealizowane.

```sh
cp rachunki.txt ~/temp/praca/zlecenia/zrealizowane/
```

5\.Przejdź do katalogu zrealizowane i zmień nazwę pliku rachunki.txt na wykonano.txt.

```sh
cd ~/temp/praca/zlecenia/zrealizowane/
mv rachunki.txt wykonano.txt
```

6\.Utwórz plik wykonano.txt wielkości 11 bajtów, następnie podziel go pliki wielkości 5 bajtów. W ten sposób otrzymasz 3 pliki.

```sh
touch wykonano.txt
atom wykonano. txt
```
_Okazuje się, że gdy wpiszemy w plik .txt ciąg znaków '1234567890' to plik ten ma  11 bajtów._

```sh
split -b 5 wykonano.txt
```
7\.Będąc w katalogu logo skopiuj powyżej otrzymane 3 pliki do katalogu dokumenty.

```sh
cd ~/temp/nauka/logo/
cp ~/temp/praca/zlecenia/zrealizowane/{xaa,xab,xac} ~/temp/praca/dokumenty/
```
8\.Będąc w katalogu dokumenty połącz skopiowane 3 pliki w plik odtworzono.txt, tak aby otrzymać plik o zawartości identycznej z wykonano.txt. Następnie plik odtworzono.txt skopiuj do katalogu wazne-sprawy.

```sh
cat xaa xab xac > odtworzono.txt
cp odtworzono.txt ~/temp/dom/wazne-sprawy/
```
9.\Będąc w katalogu wazne-sprawy sprawdź, czy są jakieś różnice w zawartości plików wykonano.txt i odtworzono.txt.

```sh
_Brak różnic. :)_
```

10.\Wyświetl kalendarz na październik 2009 r.

```sh
cal oct 2009
```


Wyświetl kalendarz na wrzesień, październik i listopad 2009 r. z miesiącami obok siebie (cal):

```sh
cal -3 oct  20
```

Wyświetl kalendarz na październik, listopad i grudzień 2009 r. w taki sposób:


```sh
cal -3 nov 2009
```
I jeszcze raz na wrzesień i październik oraz na październik i listopad 2009 r z miesiącami obok siebie:

```sh
cal -A1 sep 2009
```

```sh
cal -A1 oct 2009
```