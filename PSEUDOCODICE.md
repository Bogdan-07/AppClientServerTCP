### SERVER
Inizializzazione: Configura il Server sulla porta 12345
CICLO:
Attendi e Accetta la connessione di un Client
Crea un nuovo thread per il Client appena connesso
Gestione Thread
Apri i canali di comunicazione (BufferedReader e PrintWriter)

CICLO (Comunicazione):
Ricevi la stringa dal Client
SE la stringa è "BYE":
Invia "Arrivederci!".
INTERROMPI Ciclo.

ALTRIMENTI:
Estrai numero lati e lunghezza dal testo
Calcola Perimetro e Area
Invia la stringa con il risultato al Client

Chiudi il Socket

### Client
Tenta di stabilire la connessione con l'IP 127.0.0.1 sulla porta 12345
CICLO:
Leggi l'input digitato dall'utente
Invia la stringa al Server
SE l'input è "BYE":
Ricevi e mostra il saluto finale dal Server
INTERROMPI Ciclo.

ALTRIMENTI:
Ricevi la risposta dal Server
Mostra il risultato dei calcoli a video

Chiudi lo scanner e il Socket
