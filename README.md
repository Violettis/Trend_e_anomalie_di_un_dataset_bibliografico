# Trend_e_anomalie_di_un_dataset_bibliografico

# DOI

# Descrizione 
Il progetto consiste nell'analisi esplorativa ed esplicativa di un dataset costituito da metadati descrittivi di pubblicazioni scientifiche di tipo bibliografico.

La parte esplorativa si concentra su particolari variabili del dataset originale quali: data_pubblicazione, editori, argomenti e autori, con l'aggiunta di una nuova colonna, genere_autori. L'intento è quello di individuare il range temporale intorno a cui si attestano le pubblicazioni e la prevalenza di determinati editori, argomenti ed autori: per quest'ultimi, si fanno anche alcune considerazioni in base al genere.

Sulla base di ciò, la sezione esplicativa parte con l'analisi della rilevanza che le biblioteche e la bibliografia hanno all'interno degli argomenti; procede poi guardando ai possibili legami tra gli argomenti e i generi degli autori. Infine, l'attenzione si concentra sui due autori più prolifici per genere: Alfredo Serrai e Fiammetta Sabba. Dopo averli analizzati nel dettaglio, si confonta anche se i risultati corrispondono a quanto ottenuto nella parte esplorativa.
# Quali sono i risultati?
I dati in input sono costituiti da un file CSV contenente informazioni costituite da metadati descrittivi di pubblicazioni scientifiche di tipo bibliografico. Le variabili considerate sono:

| Variabile | Tipo |	Definizione | Esempio |
| :------- | :--- | :--------- | :------ |
|   id     |	str | ID codice identificativo rappresentato dal link wikidata.org | 	http://www.wikidata.org/entity/Q136593329 |
|titolo |str|Titolo della pubblicazione|La mia biblioteca|
|autori | str| Autore/i della pubblicazione separati da ;, con rispettivo genere tra parentesi tonde| Alfredo Serrai
|genere_autori|str| Genere dell'autore o del team di autori costituito da tre possibilità: Maschile, Femminile o Misto| Femminile
| data_pubblicazione | int| Anno della pubblicazione in numero| 1994
|argomenti|str| Argomenti della pubblicazione separati da ;|Associazione; Bibliotecario
|basi_dati|str|Banche dati da cui si sono attinte le informazioni|Scopus; DOAJ; Emerging Sources Citation Index
|doi_disponibili|str| Identificativo persistente della pubblicazione digitale per la sua ricerca sul web|10.53223/SINAPPSI_2024-01-5
|editori | str| Editore della pubblicazione| Associazione Italiana Biblioteche
|licenze_rivista|str| Licenze della rivista separate da ;|Creative Commons Attribution
|rivista|str| Rivista su cui trovare la pubblicazione|Bibliothecae.it
|edizione|int| Numero dell'edizione a cui appartiene la pubblicazione|55
|volume|int|Numero della manifestazione fisica in cui la pubblicazione si trova|135
|pagine|int| Numero di pagine della pubblicazione |19
|url_disponibili|str| URL per individuare la pubblicazione su Internet|https://aibstudi.aib.it/article/view/13415

Link al dataset: https://raw.githubusercontent.com/dhdmch/2025-2026/refs/heads/main/data/lispod/data.csv 
# Fonte dei dati 

# Metodi e strumenti 

# Responsabili 
* Fabbri, Viola
* Gaiani, Alice
# Licenza 
I dati di input e il codice di output (incluso in questo Notebook) sono rilasciati sotto licenza [CC0 1.0 Universal.](https://creativecommons.org/publicdomain/zero/1.0/)
