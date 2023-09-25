# Progetto DAPT0123 - AceDataSport
Nel vasto universo dell'analisi dati, poche discipline offrono un palcoscenico così affascinante e dinamico quanto il mondo del tennis. Il tennis è uno sport intriso di tradizione, ma allo stesso tempo in continua evoluzione. È un connubio di talento, strategia, e una dose di imprevedibilità che lo rendono affascinante per gli appassionati di sport di tutto il mondo. Ma cosa accade quando uniamo l'incredibile potenza dell'analisi dati a questo sport affascinante? Nasce una sinergia straordinaria, una fusione di dati e competenze che ci permette di svelare nuove dimensioni dell'esperienza tennistica.
Benvenuti in questo progetto di analisi dati nel tennis, un'esplorazione avvincente delle statistiche e delle dinamiche di questo sport, supportata da potenti strumenti come Microsoft Power BI. In questo viaggio, ci immergeremo nelle cifre e nei fatti che circondano il tennis professionistico, scrutando da vicino la differenza di prestazioni tra uomini e donne, e mettendo in luce l'essenza stessa delle partite e dei giocatori attraverso grafici informativi e tabelle statistiche appositamente progettate.
L'uso di Power BI, un software di visualizzazione dati all'avanguardia, ci permetterà di tradurre i dati complessi in visualizzazioni chiare e significative. Potremo esplorare le tendenze, identificare modelli e rivelare dettagli che sfuggono all'occhio non allenato. Attraverso questa potente piattaforma, avremo la possibilità di analizzare in profondità i dati del tennis, fornendo una panoramica completa delle prestazioni di giocatori e giocatrici, così come delle dinamiche delle partite.
Una delle sfide affrontate in questo progetto sarà l'analisi comparativa tra uomini e donne nel tennis professionistico. Oltre alle evidenti differenze fisiche, ciò che emerge dai dati può rivelare aspetti intriganti sulle strategie di gioco, la consistenza delle performance e la crescita del tennis femminile nell'ambito del professionismo.
Le tabelle statistiche, create appositamente per questo progetto, rappresenteranno uno strumento fondamentale per estrarre informazioni dettagliate e sintetizzare i dati in modo chiaro e accessibile. Saranno un compagno essenziale per comprendere l'andamento delle partite, le statistiche dei giocatori e le tendenze nel tennis moderno.
# 1. Report ConfrontoTennisabstract
Questo Report consente di confrontare i migliori giocatori ATP in diverse statistiche. Si trovano, statistiche sui Game, partite, Ace, set vinti e breakpoint guadagnati.


per eventi di livello Master, tornei su terra battuta o molte altre combinazioni. 

Uomini: http://www.tennisabstract.com/cgi-bin/leaders.cgi
Donne: http://www.tennisabstract.com/cgi-bin/leaders_wta.cgi .

Ho convertito questi dati in file CSV e li ho importati in questo notebook. Volevo vedere se esistono diversi "tipi" di tennisti e come questi tipi sono correlati al genere. In quanto tale, si trattava di un compito di apprendimento non supervisionato. Il set di dati è piuttosto piccolo (100 giocatori) e consiste interamente di parametri di risultato (ad esempio punti al servizio vinti) piuttosto che dati sugli aspetti fisici del gioco (ad esempio velocità del servizio), quindi potrei non avere la risoluzione necessaria per rispondere in modo esaustivo questa domanda.

Ho iniziato osservando le distribuzioni delle metriche in entrambi i set di dati. Ho rimosso le funzionalità esplicitamente associate al rango perché volevo prendere in considerazione le categorie di giocatori mentre ero cieco al rango. Ho anche rimosso alcune funzionalità ridondanti e funzionalità per le quali alcuni giocatori non disponevano di dati sufficienti.

Nella parte iniziale del progetto, ho esaminato i dati del tennis facendo una distizione tra i due sessi per capire se ci sono vari.
Tennis Abstract contiene dati sulle ultime 52 partite giocate dai migliori 50 tennisti uomini e donne.



# 2. xxxxxxx

For the purpose of the project, we consider three datasets:

<ins>Match.csv</ins>- It contains all the match level data. For eg:round, tournament, year of tournament etc. <br>
<ins>Player.csv</ins>- It contains all the details pertaining to each player. For eg: Birthday, playing hand, country etc. <br>
<ins>Stats.csv</ins>- It has all the data from all the matches played by each player. For eg: aces, break points won/ saved, rank, points etc. <br>

  Datasets have data from 2000 Aus Open - 2019 US Open for only ATP


