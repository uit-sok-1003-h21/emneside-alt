{% include navbar_open.html %}
# Installere Python, git og Jupyter på Mac

[Se video her!](https://mediasite.uit.no/Mediasite/Play/246d1f3eb5a044d8a8c8a767cb80c5941d)


## 1. Installere python 3.8.10
Før du begynner må du sørge for at du har adminrettigheter

1. Gå til [installasjonssiden for Python 3.8.10](https://www.python.org/downloads/release/python-3810/){:target="blank"}
3. Klikk på eplet->"About this mac" for å finne ut om du har intel eller apple-chip.
4. Velg filen «macOS 64-bit Intel installer» eller  «macOS 64-bit universal2 installer» avhengig av om du har intel eller ikke.
5. Velg MacOS
6. Installer "homebrew":
    1.  Følg lenken og kopier kommandoen ved å trykke på kopieringsknappen til høyre for kommandoen
    2.  Åpne kommandovinduet (Åpne finder og skriv "terminal" i søkefeltet og åpne Terminal)
    3.  Lim inn teksten du kopierte og trykk enter
4.  Gå tilbake i nettleseren til git-siden og kopier kommandoen i rødt.
5.  Lim den inn i Terminal og trykk enter
  
(Jeg har endret litt på "oppskriften" etter at videoen ble spilt inn. Det er nå lenker direkte til installasjonsidene istedet for til Google)
 
## 2. Installere git

1. Gå til [installasjonssiden for git](https://www.google.com/search?q=install+download+git){:target="blank"}
2. Velg "MacOS"
3. Åpne "Terminal" på din Mac (Søk evt. etter "Terminal" på "My Mac" i Finder)
4. Følg instruksjonene, og legg spesielt merke til at
    1. du må installere "homebrew" først, før du kan installere git
    2. Når du skal installere "homebrew" blir du bedt om et passord i terminalen. Skriv passordet ditt
  
## 3. Installere Jupyter lab

1. åpne kommandovinduet: Åpne finder og skriv "terminal" i søkefeltet og åne terminal. 
2. Skriv inn "sodu -H pip3 install jupyterlab" ("sodu -H" er for å installere det som admin, slik at du kan åpne jupyter med kommandoen "jupyter")
3. Skriv inn passord

## 4. Hente kursmateriell fra github

For å hente filene til Jupyter gjør du slik:

2. Lag en ny mappe på ditt hjemmeområde ved å skrive inn i terminalvinduet

```mkdir sok-1003```

3. Gå så inn i den mappen du har laget ved å skrive 

```cd sok-1003```
        
4. Last ned kursmateriellet ved å kopiere inn følgende kommando i kommandovinduet: 

```git clone https://github.com/uit-sok-1003-h21/notebooks/```
        
5. Filene på github kommer til å endres, og da må du oppdatere dem. Det kan derfor være lurt å ha en 
kopi av notebooks-folderen hvor du kan gjøre egne endringer som ikke overskrives når du henter oppdaterte notater.For å lage en slik kopi skriver du:
        
```cp -r notebooks notebooks_edit```
        
6. For å åpne filene i "notebooks_edit"-mappen i jupyter lab skriver du
```
cd notebooks_edit
jupyter lab
```
