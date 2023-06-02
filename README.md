<h1 align="center">Reti di Calcolatori - UNISA</h1>
<h3 align="center">Riassunto</h3>
<h3>INTRODUZIONE ALLE RETI</h3>
<br>

**ICT** --> Tecnologie per il trattamento e la trasmissione dell'informazione

\- CHE COS'é INTERNET?
- Un'infrastruttura di comunicazione che consente il trafermento di dati tra dispositivi collegati alla rete (indipendentemente dal tipo di dispositivi e dal tipo di dsti digitali che si vuole trasmettere).

Il termine **RETE** è molto generico e si applica i tantissimi ambiti
* Insieme di elementi (**NODI**) tra i quali sono definite delle relazioni (**COLLEGAMENTI**)

Una **RETE DI CALCOLATORI** connette dispositivi programmabili e può supportare applicazioni differenti e trasportare qualsiasi tipo di dati

La **COMUNICAZIONE** consente lo scambio di dati tra due dispositivi, può essere locale o remota(Tele-comunicazione) e coinvolge sia hardware che software.
Le informazioni sono rappresentate tramite i dati

**COMUNICAZIONE DATI = SCAMBIO DI DATI CHE RAPPRESENTANO L'INFORMAZIONE** <br>


La comuniazione dati avviene attraverso un mezzo trasmissivo

<h4>SISTEMA DI COMUNICAZIONE:</h4>

* MESSAGGIO
* MITTENTE
* DESTINATARIO
* MEZZO TRASMISSIVO
* PROTOCOLLO

![sistema telecomunicazione](src/sistema_di_comunicazione.png)


<h4>TIPO DI CONNESSIONE:</h4>

* **PUNTO PUNTO**
![punto punto](src/punto-punto.png)

* **MULTIPUNTO**
![ulti punto](src/multi-punto.png)


<h4>COMUNICAZIONE:</h4>

* **UNIDIREZIONALE**
![unidirezionale](src/unidirezionale.png)

* **BIDIREZIONALE ALTERNATA**
![bidirezionale alternata](src/bidirezionale-alternata.png)

* **BIDIREZIONALE (FULL DUPLEX)**
![bidirezionale](src/bidirezionale.png)

La **connessione diretta** (sia punto punto che multipunto) è adatta solo a reti piccole perché il numero di collegamenti è limitato al numero di porte presenti nel nodo, e non è **scalabile**

La **connessione "indiretta"** permette di creare reti "grandi" ed economiche
img
![nodi di commutazione](src/nodi-commutazione.png)
É composta da 2 tipi di nodi
* Terminali
* Commutazione
	* collegamenti ad almeno 2 linee
	* hanno la funzione di smistare il traffico
	* non ci sono utenti su questi nodi


<h3>RETI A COMMUTAZIONE</h3>

L' insieme di switch costituisce una rete a commutazione:
* La rete utilizzata per creare connessioni tra diversi utenti
* Le risorse della rete sono condivise dai vari utenti
* La rete commuta tra una comunicazione e l'altra
É una soluzionepiù economica e scalabile che consente un uso efficiente della rete
2 tecniche di commutazione:
* CIRCUITO (telefonico)
* PACCHETTO (postale)

<h3>CLASSIFICAZIONE DELLE RETI</h3>
La classificazione avviene in base all'area coperta (variano le scelte tecnologiche e progettuali)

<h4>LAN (Local Area Network)</h4>

* Copre l'area di un edificio o di un campus
* es. comunicazione ad eccesso multiplo con doppino telefonico

<h4>MAN (Metropolitan Area Network)</h4>

* Copre l'area di una città
* Comunicazione indiretta con fibra ottica

<h4>WAN (Wide Area Network)</h4>

* Copre l'area di una regione o Nazione
* Comunicazione indiretta con fibra ottica o trasmissione a microonde (es. satelliti)




<h3>COMUNICAZIONE UNIVERSALE</h3>
Ogni nodo può comincare solo con altri nodi connessi alla stessa rete
Gli utenti richiedono un servixio di comunicazione universale(connessione con ogni altro utente indipendentemente dalla posizione , dal tipo di rete e del tipo di software utilizzato)
Come si ottiene? ↓

<h3>INTERNETWORKING</h3>
Una interrete (Internet) è una rete di reti

* I suoi nodi sono reti (possibilmete di tipo diverso) -> definizione Ricorsiva
* Le reti sono collegate tramite router (Gateway)
![internetworking](src/internetworking.png)



L'internetworking consente di comunicare con utenti collegate ad altre reti
Il software d i rete rende trasparente all'utente le differenze tra reti fisiche
Il software applicativo è indipendente dalla tecnologia hardware utilizzata (lo stesso programma può essere usato su qualsiasi rete)
**Internet** è l'esempio più conosciuto di inter-rete. Ci sono modi di descrivere questo sistema estremamente complesso:
+ in termini di suoi componenti
+ in termini di servizi offerti agli utenti



<h3>HOSTS</h3>
Sono dispositivi in grando di eseguire elaborazioni e collegati alla rete (PC, SERVER, LAPTOP, SMARTPHONE) su cui operano gli utenti (end-system). Vengono utilizzati per eseguire applicazini di rete.


<h3>LINEE DI COMUNICAZIONE</H3>

Linee su cui viagiano i dati. Sono mezzi fisici --> conduttori. Mezzi diversi hanno tassi di **(Larghezza di banda)** trasmissione diversi. Le linee più comuni: il doppino, cavo coassiale, fibra ottica, wireless, satellite.




<h3>DISPOSITIVI DI COMMUTAZIONE</H3>

Permettono la comunicazione indiretta (collegamento tra dispositivi per mezzo di altri dispositivi intermediari come ad esempio i router)

2 Categorie (entrambe smistano pacchetti sulla base dell'indirizzo di destinazione)

* **SWITCH:**
	* Consente comunicazioni tra 2 nodi della stessa rete
* **ROUTER:**
	* Smista i pacchetti tra nodi di rete diverse	


<h3>COME AVVIENE LA TRASMISSIONE?</H3>
	- Spedendo i Pacchetti (con dim. MAX e dim. STANDARD)
	- Bisogna conoscere l'indirizzo di destinazione
	- Se la dimensione del pacchetto è > della dim. MAX, il messaggio viene diviso su più pacchetti che vengono inviati, ognuno dei quali conterrà un blocco di dati. Ogni pacchetto viene trattato in modo indipendente dagli altri (possono fare strade diverse)
	-Il destinatario deve ricostruire il messaggio originale

	Nel passaggio da una rete all'altra il formato dei dati può dipendere dalla rete su cui viaggiano

Gli host non accedono direttamente alla rete internet (troppo costoso), ma accedono ai servizi di un **ISP** (Internet Service Provider) cioé aziende o enti che smistano i pacchetti e li inviano tramite Internet.
- Gli **ISP** sono interconnessi e organizzati gerarchicamente
	- Locali
	- Regionali
	- Nazionali
	- Internazionali / Globali


![ISP](src/ISP.png)

La gestione degli ISP avviene tramite un network **Access Point(NAP)** ovvero una sta za fisica in cui ci sono diversi router che consentono lo scambio di Pacchetti tra ISP differenti

<h3>PERCORSI</h3>

- Gli ISP sono autonomi nella gestione della loro rete, ma per garantire l'interoperabilità, devono accodarsi per utilizzare gli stessi **PROTOCOLLI** per l'invio, l'inoltro e la ricezione dei Pacchetti.
- Esisono centinaia di protocolli Internet -> definiti come **TCP/IP** dal nome dei 2 protocolli principali.
- I protocolli **STANDARD** vengono accettati da tutti gli utilizzaotri della rete.
- Gli Standard di Internet sono definiti dall'IETF, definiti come RFC(documenti testuali che danno una descrizione funzionale su cosa deve fare il protocollo e come deve funzionare)
**COME NASCE UN RFC?**
- Si propone un "Draft di Internet", se approvato diventa un RFC

**ALTRI STANDARD**
- Definiti da altri enti
- IEEE definisce gli standard reativi a reti LAN/MAN;
	- commissione 802 ha definito certi standard con nome 802.xx;
	- comprendono Ethernet(802.3), Wi-Fi(802.11);


<h3>INTERNET COME PIATTAFORMA DI SERVIZI</h3>

Internet fornisce servizi alle applicazioni (social, messaggistica istantanea, ecc). Queste applicazioni sono dette **APPLICAZIONI DISTRIBUITE**. Le Applicazioni distribuite sono esclusivamente eseguite sugli host. Router e Switch contribuiscono alla trasmissione dei dati ma mai intervengno nell'esecuzione dell'Applicazione.
- Un'Applicazione distribuita consiste di diversi moduli software in esecuizione su host differenti. (possono essere scritti anche in linguaggi di programmazione differenti).
- Il sistema operativo di un host collegato alla Rete fornisce un **API**: 
	- É un insieme di regole








	
	 

<a href="https://www.buymeacoffee.com/leonardospadoni"> <img align="left" src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" height="50" width="210" alt="leonardospadoni" /></a></p><br><br>
