# COVID-19 Emilia Romagna
Un flow di [Node-RED](https://nodered.org/) con espressioni [JSONata](https://jsonata.org/) per convertire i dati della [Protezione Civile](https://github.com/pcm-dpc/COVID-19) relativi alle _province dell'Emilia-Romagna_ nel formato accettato da [Flourish](https://bit.ly/covid19er).
## Dati
### Link
- dati graficati su [bit.ly/covid19er](https://bit.ly/covid19er)
- dati in formato JSON su [bit.ly/covid19er-raw](https://bit.ly/covid19er-raw)
### Elenco
- **assoluto**: totale tamponi positivi;
- **relativo**: percentuale tamponi positivi su abitanti;
- **variazione**: variazione tamponi positivi da giorno precedente.
## Requisiti
### Software
Per lanciare il programma è necessaria una versione sufficientemente recente di [Docker](https://docs.docker.com/get-docker/).
### Ambiente
Aggiungi un file `.env` con le seguenti variabili d'ambiente:
- `VOLUME_DATA` = il percorso dell'host dove persistere il flow e gli altri dati di _Node-RED_
- `VOLUME_RESULT` = il percorso dell'host dove persistere il risultato del programma
- `PORT` = la porta su cui sarà visibile il programma su _localhost_ (opzionale, se non specificato è **1880**)
## Avvio
Per lanciare il programma apri il terminale nella directory del progetto ed esegui il seguente comando:
```docker-compose up -d```
