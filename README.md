1)  GOAL DEL SISTEMA
Sorteat è un'applicazione progettata per ridurre lo spreco alimentare in contesti domestici condivisi e non (coinquilini, famiglie, chi vive da solo) fungendo da "cucina virtuale intelligente" che risolve il carico cognitivo di pianificazione e facilita la comunicazione tra membri. La value proposition di Sorteat è “Handling all the thinking, so you can focus on the eating” perché vogliamo restituire ai nostri utenti il piacere del cibo, senza il peso dei pensieri.

PRINCIPIO GUIDA
Il sistema è progettato per eliminare ogni pensiero e azione superflua dall'utente, automatizzando decisioni ripetitive e presentando solo informazioni rilevanti al momento giusto.

OBIETTIVI SPECIFICI
a) Ridurre lo spreco alimentare evidenziando prodotti in scadenza e suggerendo ricette basate su ingredienti disponibili
b) Facilitare la gestione condivisa dell'inventario domestico con sistema di proprietà privata/comune
c) Motivare comportamenti anti-spreco attraverso metriche economiche che mostrano quanto si spende e quanto si spreca



2) UTENTI TARGET

a) PROFILO PRIMARIO giovani adulti coinquilini
Età: 22-35 anni
Contesto: studenti universitari, giovani professionisti
Situazione abitativa: appartamenti condivisi con 2-4 coinquilini
Competenza tecnologica: media-alta
Motivazioni:
Risparmiare denaro sul cibo
Gestire in modo equo le spese condivise
Evitare conflitti con i coinquilini e avere una comunicazione più semplice per quanto riguarda il cibo 
Pianificare pasti senza stress



b) PROFILO SECONDARIO nuclei familiari
Contesto: coppie o piccole famiglie con stile di vita dinamico
Caratteristiche: scarso tempo per pianificazione, attenzione al budget
Esigenze: ottimizzare spesa alimentare, ridurre sprechi, bilanciare contributi

PAIN POINTS RISOLTI
"Non sapevo che il latte era scaduto" → Sistema di alert automatici per scadenze
"Ho comprato cose già presenti in casa" → Inventario condiviso accessibile
"Non so cosa cucinare con quello che ho" → Suggerimenti ricette basati su inventario
"Chi mi deve i soldi della spesa?" → Bilancio automatico con tracciamento



 3) CONTESTO D'USO

SCENARIO TIPICO
Un appartamento condiviso da 3 coinquilini (Mariia, Giorgia, Luca) che:
Condividono frigo, dispensa e freezer
Hanno sia prodotti comuni che privati
Alternano chi fa la spesa
Cucinano sia individualmente che insieme
Vogliono dividere equamente le spese

MOMENTI DI INTERAZIONE

a) A casa
controllo veloce dei prodotti in scadenza per sapere cosa mangiare quel giorno
ricerca di ispirazione per colazione / pranzo / cena 
pianificazione giornaliera / settimanale dei pasti
aggiunta della spesa appena fatta all’inventario

b) Al supermercato
consultazione della lista della spesa condivisa
scansione scontrino per aggiornamento dell’inventario
controllo della presenza o meno di un prodotto nell’inventario

c) In mobilità
aggiunta rapida articoli alla lista spesa
notifiche push per prodotti in scadenza

DISPOSITIVI
Primario: smartphone (iOS/Android)
Modalità: portrait, touch interface






4) TASK IMPLEMENTATI

TASK 1: verificare la necessità di acquisto di un ingrediente

Obiettivo: L'utente deve essere in grado di controllare rapidamente se un ingrediente è già disponibile in casa (e in quale quantità) prima di aggiungerlo alla lista spesa / comprarlo, evitando acquisti doppi.

Scenario: Luca è al supermercato e si trova davanti al banco frigo. Il suo dilemma è sempre lo stesso: "Compro il latte o no?". Se non lo compra, c'è un'alta probabilità di non poter fare colazione l'indomani, costringendolo a uscire di nuovo solo per quello, a iniziare la giornata già di malumore o a fare colazione al bar. Se lo compra, rischia di trovarne un'altra confezione a casa, sprecando quei due euro che, sommati a tutte le altre volte, iniziano a pesare sul suo budget da studente. Per fortuna, Luca si ricorda di avere l’app Sorteat e quindi va subito a controllare la presenza o meno del latte in casa.

FLUSSO DETTAGLIATO

a) OPZIONE A: RICERCA RAPIDA
1. L'utente apre l'app → visualizza Inventario
2. Nella barra superiore, tap su tab 🔎 Cerca (nel visual switcher)
3. Appare campo di ricerca con placeholder _"Cerca prodotto..."_
4. Digita "Latte" → risultati filtrati in tempo reale
5. Visualizza prodotto trovato:
Emoji: 🥛
Nome: Latte Intero
Quantità: 0.5 L 
Scadenza: "2 giorni" (badge arancione)
Proprietà: Nessun lucchetto → prodotto suo / comune (può usarlo)
6. Decisione:
Se quantità sufficiente → Non aggiunge alla spesa
Se quantità insufficiente → Procede con aggiunta della quantità necessaria

b) OPZIONE B: NAVIGAZIONE PER UBICAZIONE
1. Dall'Inventario, sa che il latte è in frigo
2. Tap su tab 🍳 Frigo (nel visual switcher)
3. Scorri prodotti organizzati per categoria
4. Trova sezione "LATTICINI E UOVA" (etichetta con linee divisorie)
5. Visualizza card latte con stesso dettaglio (emoji, nome, quantità, scadenza)

AZIONE DI FOLLOW-UP: AGGIUNTA ALLA LISTA SPESA
7. Se decide che serve comprare latte dall'Inventario: Tap su icona carrello (in alto a destra)
8. Si apre “Spesa”
9. Tap su "+"
10. Form rapido:
Nome: "Latte" 
Quantità: 2
Unità: L
11. Tap "Aggiungi" → Articolo aggiunto con badge carrello aggiornato (1)
CASO SPECIALE: PRODOTTO PRIVATO
Se il latte trovato ha il “lucchetto 🔒” e avatar di un altro coinquilino: significa che il prodotto è privato di un altro coinquilino, non può usarlo senza permesso
Decisione 1: deve comprare latte proprio → aggiunge a lista spesa
Decisione 2: tap sul prodotto → "Chiedi a [nome coinquilino]" → notifica il coinquilino



TASK 2: scegliere cosa cucinare

Obiettivo: L'utente deve poter scegliere una ricetta da preparare, considerando gli ingredienti disponibili in casa e i prodotti in scadenza da consumare urgentemente. 

Scenario: È sabato mattina e Mariia va ad un mercato agricolo di quartiere.  Il suo sguardo viene catturato da una bancarella con dei funghi porcini freschissimi e profumati. Immediatamente, nella sua mente si forma un'immagine vivida: un risotto ai funghi perfetto, cremoso. Si sente ispirata. È esattamente il tipo di esperienza culinaria autentica che vorrebbe vivere più spesso. L'impulso di acquistarli è fortissimo. Ma subito dopo, un'ondata di incertezza frena il suo entusiasmo. Inizia il solito dialogo interiore: "Ok, compro i funghi. Ma a casa ho il riso Carnaroli, o solo quello Basmati? E il brodo vegetale? Sicuramente non ce l'ho. E il parmigiano? Forse è finito... O era la scamorza?". Tira fuori il telefono e si ricorda che può tranquillamente controllare se ha il necessario dall’app Sorteat. 

FLUSSO DETTAGLIATO

ESPLORAZIONE RICETTE DISPONIBILI
1. L’utente apre l’app → dalla Navigation Bar in basso, tap sull'icona Ricette
2. Si apre la pagina Ricette con due sezioni:
Sezione 1: Meal planner (con doppia vista: calendario e lista)
Sezione 2: “Ispirazioni per [momento corrente della giornata: colazione / pranzo / cena]”

3. Decide di esplorare le ispirazioni per la cena 
→ Card ricette con immagine, nome, tempo, persone
“Pasta al pomodoro” - 30 min ← “ah la ricetta usa i pomodori”
“Risotto ai funghi” - 45 min

4. Tap su card "Risotto ai funghi" → Visualizzare dettaglio ricetta
5. Si apre modale/pagina “Pianifica evento” con:
Emoji piatto (header)
Nome: Pasta al Pomodoro
Info: tempo | porzioni
Ingredienti necessari:
Riso Carnaroli (400g) - disponibile (badge grigio)
Parmigiano (100g) - disponibile (badge arancione perché scade tra 2 giorni)
Aglio (2 spicchi) - disponibile 
Funghi porcini - mancanti (badge rosso e scritta)
Olio (10 ml) - mancante, “Chiedi a Luca”


6. L'utente ha 3 opzioni:

Opzione 1: cucinare ora
Tap sul pulsante “Pianifica"
Ricetta viene aggiunta al pasto coerente con l’ora corrente 

Opzione 2: pianificare per dopo
Drag&drop: l’utente trascina la ricetta desiderata nello slot corrispondente nel Meal Planner

Opzione 3: aggiungere ingrediente mancante / chiedere ingrediente a coinquilino
Nota che manca l’olio
Tap su badge “Chiedi a Luca” / aggiungi ingrediente lista della spesa



TASK 3: aggiornare l'inventario condiviso con la nuova spesa

Obiettivo: L'utente deve poter aggiungere rapidamente i prodotti acquistati all'inventario condiviso dopo aver fatto la spesa, utilizzando scansione scontrino o inserimento manuale.

Scenario: Giorgia torna dal supermercato con la spesa settimanale. Ha comprato 8 prodotti e vuole aggiornarli nell'inventario condiviso il più velocemente possibile. Prova prima la scansione scontrino (innovativa), poi aggiunge manualmente un prodotto fresco comprato al mercato (senza scontrino).

FLUSSO DETTAGLIATO

Parte A: accesso funzione aggiornamento
1. L'utente apre l'app → naviga a Inventario
2. Vede FAB "+"** verde fisso in basso a destra (floating action button)
3. Tap su FAB "+"
4. Si apre pagina "Aggiorna Inventario" con 2 opzioni grandi in card:

Card 1: Scansiona scontrino
Card 2: Inserimento manuale

Parte B: scansione scontrino (flusso rapido)
5. Tap su “Scansiona scontrino”
6. Si apre Camera View (simulata):
Mirino centrale con cornice
Overlay guida: "Inquadra il tuo scontrino"
Pulsante scatto centrale (circolare, verde)

7. Tap su Scatta foto (simula foto)
8. Loading Screen (2-3 secondi):
9. Si apre “Revisione Prodotti” con lista prodotti riconosciuti (prodotti mock)


→ Interazioni disponibili in revisione:

10. Modifica prodotto:
Tap su qualsiasi campo → editing inline

11. Rimuovi prodotto:
Icona cestino a destra della card prodotto

13. Imposta scadenza (consigliato):
Tap su data → si apre Date Picker
Seleziona giorno → campo aggiornato

14. Toggle proprietà:
Tap su toggle "Comune/Privato"
Possibilità di indicare con chi viene condiviso

Conferma e salvataggio:
15. In fondo alla lista, pulsante “Aggiungi all'inventario”
16. Tap su “Aggiungi all'inventario”
17. Redirect automatico a Inventario → vede nuovi prodotti nelle rispettive ubicazioni

Parte C: Inserimento manuale
19. Giorgia si ricorda: ha comprato basilico fresco al mercato (no scontrino)
20. Dall'Inventario, tap di nuovo su FAB "+"
21. Questa volta sceglie “Inserimento manuale”
22. Si apre Form di Inserimento con campi vuoti:
Nome Prodotto (obbligatorio)
Quantità(obbligatorio)
Numero: 1
Unità (dropdown): mazzo (opzioni: kg, g, L, ml, pz, mazzo, spicchio...)
Prezzo (opzionale) 
Proprietà (obbligatorio)
Scadenza (consigliato) 

23. Tap su “Aggiungi” 
24. Scelta della categoria del prodotto appena aggiunto
25. Prodotto aggiunto 
26. Tap su “Conferma 1 prodotto”
27. Visualizzazione del prodotto nell’Inventario

Nota importante: Una volta inseriti i prodotti nell'Inventario si cancelleranno automaticamente dalla lista della spesa. La sezione “Spesa” è pensata, per adesso, come aiuto promemoria per l’utente, che può sbarrare i prodotti via dalla lista senza ché questi vengano aggiunti all’Inventario.



5) INDICAZIONI PER LA VALUTAZIONE

COSA L'UTENTE DOVREBBE ESSERE IN GRADO DI FARE

Navigazione base
- Spostarsi tra le 4 sezioni principali tramite Navigation Bar: 
Home / Inventario / Ricette / Spazio
- Tornare indietro usando frecce in-app (no browser back)
- Riconoscere sezione attiva (icona filled + colore verde)

Gestione inventario
- Visualizzare tutti i prodotti organizzati per ubicazione (Frigo / Dispensa / Freezer)
- Cambiare vista tramite visual switcher (4 tab emoji)
- Identificare prodotti urgenti nell'area “Da consumarsi subito”
- Aprire dettaglio prodotto con tap singolo
- Modificare quantità/scadenza di prodotti comuni o propri
- Eliminare prodotti con conferma
- Richiedere permesso per prodotti privati altrui
- Aggiungere nuovi prodotti tramite scansione o manuale

Spesa
- Visualizzare articoli nella lista spesa
- Aggiungere articoli alla lista
- Spuntare articoli acquistati
- Vedere badge numero articoli su icona carrello

Ricette
- Navigare sezione ricette
- Visualizzare ricette disponibili
- Vedere ingredienti richiesti
- Pianificare pasti nel calendario settimanale

Bilanci
- Consultare metriche economiche personali (Home)
- Vedere impatto collettivo del gruppo (Bilancio)
- Verificare saldi con ogni coinquilino
- Saldare debiti/crediti con conferma
- Consultare storico transazioni

COSA L'UTENTE NON PUÒ FARE (LIMITAZIONI)

Limitazioni tecniche del prototipo
- No backend reale: tutti i dati sono mock/localStorage, non persistenti tra sessioni
- No autenticazione: utente corrente è fisso (Mariia), no login/logout
- No notifiche push reali: tutte le notifiche sono simulate tramite toast
- No OCR reale: scansione scontrino usa dati predefiniti
- No ricerca avanzata: ricerca prodotti/ricette limitata a matching semplice
- No gestione account: non si può modificare profilo, aggiungere/rimuovere membri (oltre onboarding)
Funzionalità Non Implementate
- Modifica membri dello spazio (solo visualizzazione)
- Integrazione calendario esterno
- Scan barcode prodotti
- Condivisione lista spesa via link
- Calcolo effettivo / reale del bilancio 

CREDENZIALI E DATI DI TEST
Utente corrente (fisso): Mariia
Altri membri dello spazio: Giorgia, Luca
