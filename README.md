# Trend_e_anomalie_di_un_dataset_bibliografico

# DOI
[10.5281/zenodo.19675959] 
# Descrizione 
Il progetto consiste nell'analisi esplorativa ed esplicativa di un dataset costituito da metadati descrittivi di pubblicazioni scientifiche di tipo bibliografico.

La parte esplorativa si concentra su particolari variabili del dataset originale quali: data_pubblicazione, editori, argomenti e autori, con l'aggiunta di una nuova colonna, genere_autori. L'intento è quello di individuare il range temporale intorno a cui si attestano le pubblicazioni e la prevalenza di determinati editori, argomenti ed autori: per quest'ultimi, si fanno anche alcune considerazioni in base al genere.

Sulla base di ciò, la sezione esplicativa parte con l'analisi della rilevanza che le biblioteche e la bibliografia hanno all'interno degli argomenti; procede poi guardando ai possibili legami tra gli argomenti e i generi degli autori, analizzando anche un caso particolare. Infine, l'attenzione si concentra sui due autori più prolifici per genere: Alfredo Serrai e Fiammetta Sabba. Dopo averli analizzati nel dettaglio, si confonta anche se i risultati corrispondono a quanto ottenuto nella parte esplorativa.

# Quali sono i risultati?
Le conclusioni sui risultati ottenuti, contenuti nel Jupyter Notebook, possono essere divise sulla base dell'analisi esplorativa e esplicativa.

Dall'analisi esplorativa le conclusioni evidenziano:
* Una copertura temporale ampia, dal 1816 al 2025, con un notevole aumento delle pubblicazioni negli ultimi 15 anni; il picco massimo è stato raggiunto nel 2020.
* L'editore più ricorrente è l'Associazione Italiana Biblioteche, che conta oltre 500 pubblicazioni.
* L'argomento maggiormente trattato è quello "Bibliotecario", ripetuto oltre 110 volte.
* Non notiamo una significativa distinzione di genere: gli uomini, da soli o in team dello stesso genere, sembrano pubblicare più delle donne per pochi punti percentuali. Inoltre, i team misti non sono popolari: compongono meno dell'8% dei casi totali.
* L'autore più prolifico è Alfredo Serrai, con 61 pubblicazioni, seguito da Fiammetta Sabba, con 25.

L'analisi esplicativa ha determinato che:
* La "Biblioteca" e le sue accezioni sono tra i temi maggiormente trattati, ricoprendo poco più del 22% del totale.
* Sembrano esserci argomenti più trattati da un genere rispetto all'altro, ma non in percentuali significative: gli stessi argomenti vengono analizzati tanto dagli uomini quanto dalle donne, ma i primi lavorano con maggior frequenza sul tema della bibliografia rispetto alle donne, mentre queste ruotano di più intorno alle biblioteche. Nei team misti si ripete quanto stabilito per uomini e donne, se non per un nuovo argomento "lavoro" che si distingue dal resto.
* Approfondendo i generi appuriamo che: gli uomini, come autori singoli, pubblicano più che le autrici donna, ma possiamo vedere che quest'ultime sono maggiormente propense a formare team dello stesso sesso. Inoltre, sommando le percentuali di Uomini e Donne, otteniamo come risultato 8%, che corrisponde alla portata degli articoli scritti da team misti: quindi, non si rileva più comune scrivere in team dello stesso genere rispetto a gruppi di lavoro misti, o viceversa. In totale, il 15.7% degli articoli è stato scritto da più mani.

Focalizzandoci sui due autori più prolifici per ciascun genere, si scopre che:
* Alfredo Serrai
  * Non partecipa a team di lavoro, prediligendo la pubblicazione come unico autore e rispecchiando l'andamento del genere maschile;
  * L'anno in cui pubblica di più, il 2015, non corrisponde all'anno più prolifico a livello generale;
  * L'argomento di cui scrive maggiormente è la "Storia della bibliografia", in linea con il  dataset generale;
  * L'editore col quale egli pubblica più frequentemente è l'Università di Bologna, ben 60 scritti su 61; non si lega quindi all'editore più prolifico del database, l'Associazione Italiana Biblioteche, con cui egli pubblica un solo articolo.
* Fiammetta Sabba
  * Partecipa a pubblicazioni realizzate in team, dimostrando l'andamento del genere femminile maggiormente portato alla scrittura a più mani, ma non ha una particolare propensione per team omogenei o eterogenei per sesso;
  * L'anno in cui pubblica di più è il 2016, dimostrandosi anch'essa non in linea con l'analisi generale; nemmeno l'anno in cui prende maggiormente parte a pubblicazioni in team, il 2021, corrisponde;
  * L'argomento di cui pubblica di più è la "Storia della bibliografia", allineandosi a Serrai ma non alla tendenza del suo genere di appartenenza. Per quanto riguarda le pubblicazioni in team misti, riprende gli argomenti comunemente trattati da questa categoria, ma non scrive dell'eccezione "lavoro" precedentemente individuata.
  * Anche per lei l'editore più ricorrente è l'Università di Bologna, non partecipando al trend generale dell'Associazione Italiana Bibblioteche, ma coincide con il comportamento di Serrai. Anche quando è in team l'editore più frequente non è l'Associazione Italiana Biblioteche.
Le indagini, basate sulle scelte effettuata, hanno prodotto delle interessanti riflessioni sull'operato di alcuni autori e sugli argomenti maggiormente studiati; non hanno, però, evidenziato trend consistenti né anomalie consistenti all'interno del database.

# Fonte dei dati 
I dati in input sono costituiti da un file CSV contenente informazioni costituite da metadati descrittivi di pubblicazioni scientifiche di tipo bibliografico. Le variabili considerate sono:

| Variabile | Tipo |	Definizione | Esempio |
| :------- | :--- | :--------- | :------ |
|   id     |	str | Codice identificativo rappresentato dal link wikidata.org | 	http://www.wikidata.org/entity/Q136593329 |
|titolo |str|Titolo della pubblicazione|La mia biblioteca|
|autori | str| Autore/i della pubblicazione separati da ;| Alfredo Serrai
|genere_autori|str| Genere dell'autore o del team di autori con tre possibilità: Maschile, Femminile o Misto| Femminile
| data_pubblicazione | int| Anno della pubblicazione in numero| 1994
|argomenti|str| Argomenti della pubblicazione separati da ;|Associazione; Bibliotecario
|basi_dati|str|Banche dati da cui si sono attinte le informazioni|Scopus; DOAJ; Emerging Sources Citation Index
|doi_disponibili|str| Identificativo persistente della pubblicazione digitale per la sua ricerca sul web|10.53223/SINAPPSI_2024-01-5
|editori | str| Editore della pubblicazione| Associazione Italiana Biblioteche
|licenze_rivista|str| Licenze della rivista separate da ;|Creative Commons Attribution
|rivista|str| Rivista su cui trovare la pubblicazione|Bibliothecae.it
|edizione|int| Numero dell'edizione a cui appartiene la pubblicazione|55
|volume|int|Numero della manifestazione fisica in cui la pubblicazione compare|135
|pagine|int| Numero di pagine della pubblicazione |19
|url_disponibili|str| URL per individuare la pubblicazione su Internet|https://aibstudi.aib.it/article/view/13415

I dati originali sono stati forniti dal professore Sebastian Barzaghi e recuperati dall'apposito link, contenente il dataset, caricato su GitHub.

Link al dataset: https://raw.githubusercontent.com/dhdmch/2025-2026/refs/heads/main/data/lispod/data.csv

# Metodi e strumenti 
Il progetto è stato sviluppato in un ambiente Google Colab utilizzando il linguaggio di programmazione Python. Gli strumenti principali utilizzati per la manipolazione, l'analisi e la visualizzazione dei dati sono state due librerie: Pandas e Matplotlib Pyplot.
Le operazioni hanno incluso:
* Caricamento e ispezione dei dati (alcune di queste: pd.read_csv, df.info(), df.describe())
* Bonifica e normalizzazione dei dati (alcune di queste: df.duplicated.value_counts(), df.drop(), .astype(), pd.to_numeric(errors=coerce), .explode().dropna())
* Creazione di nuove variabili calcolate (alcune di queste: genere_autori, argomenti_separati, serrai_pubblicazioni)
* Nell'analisi esplorativa si trovano aggregazioni (come: .value_counts() e visualizzazioni tramite grafici a barre orrizzontali (plot.barh()) o a torta (plot.pie())
* Nell'analisi esplicativa si è sviluppata una narrativa concentrata su di generi, argomenti e autori specifici per confrontarli ai trend generali

# Responsabili 
* Fabbri, Viola
* Gaiani, Alice

# Licenza 
I dati di input e il codice di output (incluso in questo Notebook) sono rilasciati sotto licenza [CC0 1.0 Universal.](https://creativecommons.org/publicdomain/zero/1.0/) 
