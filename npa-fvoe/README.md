# Descrizione
Il repository contiene la documentazione tecnica dei servizi di cooperazione applicativa per integrarsi con la Nuova Piattaforma Appalti (NPA) messa a disposizione sall'’Autorità Nazionale Anticorruzione (ANAC)

# Documentazione
## Specifiche interfacce
 - Il [file YAML](/npa-fvoe/docs/specifiche-interfacce/specifiche-servizi-appalto.yaml) relativo alle specifiche dei servizi esposti dalla NPA per la gestione del Ciclo di vita dell'Appalto
 - Il [file YAML](/npa-fvoe/docs/specifiche-interfacce/specifiche-servizi-fvoe-fva.yaml) relativo alle specifiche dei servizi esposti dalla NPA per la gestione del Fascicolo Virtuale dell'Operatore Economico e del Fascicolo Virtuale dell'Appalto
 - Il [documento](/npa-fvoe/docs/specifiche-interfacce/documento-specifiche-servizi-npa.md) di sintesi di Specifica delle Interfacce redatto utilizzando il linguaggio di markup Markdown

## Modello dati
Il [file YAML](/npa-fvoe/docs/modello-dati/modello-dati-npa.yaml) contenente la definizione dinamica del modello dati referenziato nelle specifiche dei servizi esposti dalla NPA. *Esempio*:
 ```shell
 StatoLottoEnum:
   $ref: 'https://github.com/anticorruzione/npa-fvoe/docs/modello-dati/modello-dati-npa.yaml#/components/schemas/StatoLottoEnum'
 ```

## Immagini
Le immagini che rappresentano il contesto, i flussi di interoperabilità e le transizioni di stato per l'intero Ciclo di Vita dell’Appalto sono
consultabili nella cartella [immagini](/npa-fvoe/docs/immagini/).

## Diagrammi drawio
I diagrammmi di contesto, di sequenza e di stato per l'intero Ciclo di Vita dell'Appalto sono consultabili nella cartella [diagrammi-drawio](/npa-fvoe/docs/diagrammi-drawio/) e, sono stati disegnati mediante l'utilizzo di [Draw.io](https://www.draw.io/).

## Orchestratore
La complessità della verifica durante l'acquisizione delle schede dati è gestita dal componente NPA di orchestrazione che, tramite il suo motore di regole, ha il compito di:
- verificare se la scheda dati passata in input è coerente con lo stato dell’Appalto
- effettuare una validazione sintattica dei dati di input

Lo schema delle regole di acquisizione di una schede dati è consultabile nella cartella [orchestratore](/npa-fvoe/docs/orchestratore/).

# Domande
Il canale di comunicazione con ANAC è rappresentato dall'apposita sezione [Issues](https://github.com/domaltomare/YAML/issues) nella quale sarà possibile inserire una richiesta.

# Disclaimer
L’Autorità Nazionale Anticorruzione è sollevata da eventuali responsabilità dovute a:
- mancata risposta a richieste pervenute o di competenza di organizzazioni esterne.
- richieste pervenute al di fuori dell'unico canale di comunicazione con ANAC rappresentato dalla sezione [Issues](https://github.com/domaltomare/YAML/issues)
