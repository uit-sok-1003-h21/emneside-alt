{% include navbar_open.html %}
# Installere Python, git og Jupyter på Windows

1. Installere python 3.8.10
    1. Google «install python 3.8.10»
    2. Velg «3.8.10»
    3. Velg filen «Windows x86-64 executable installer»  
    4. Installer for alle brukere (krever elevering/admin login) og **hak av for å legge til "PATH"**. 
  
2. Installere git
    1. Google "install git"
    2. Velg "Downloads - Git"
    3. Last ned og installer for alle brukere (krever elevering/admin login)
  
3. Installere Jupyter lab
    1. åpne kommandovinduet: trykk på windowsknappen, skriv "cmd" og start "Command Promt"/"Ledetekst". 
    2. Skriv inn `pip install jupyterlab`

## Hente kursmateriell fra github

For å hente filene til Jupyter gjør du slik:

2. Lag en ny mappe på ditt hjemmeområde ved å skrive inn i terminalvinduet

```mkdir sok-1003```

3. Gå så inn i den mappen du har laget ved å skrive 

```cd sok-1003```
        
4. Last ned kursmateriellet ved å kopiere inn følgende kommando i kommandovinduet: 

```git clone https://github.com/uit-sok-1003-h21/notebooks/```
        
5. Filene på github kommer til å endres, og da må du oppdatere dem. Det kan derfor være lurt å ha en 
kopi av notebooks-folderen hvor du kan gjøre egne endringer som ikke overskrives når du henter oppdaterte notater.For å lage en slik kopi skriver du:
        
```xcopy notebooks notebooks_edit```
        
6. For å åpne filene i "notebooks_edit"-mappen i jupyter lab skriver du
```
cd notebooks_edit
jupyter notebook
```
