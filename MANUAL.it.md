# Loop Gizmo — Manuale d'uso

**Versione 2.0** · 🇬🇧 [English version](MANUAL.md)

▶ **Versione live: [https://droogia.github.io/loop-gizmo/](https://droogia.github.io/loop-gizmo/)**

Loop Gizmo è una loop station a 6 tracce che funziona nel browser. Segue il flusso di lavoro di un looper hardware da tavolo: registri una frase, ci sovrapponi altre parti, distribuisci le parti su tracce separate, aggiungi una base ritmica di batteria e modelli tutto con gli effetti in tempo reale.

I nomi dei comandi (pulsanti, manopole, pagine del display) sono riportati in inglese, esattamente come appaiono sul pannello.

---

## Indice

1. [Per iniziare](#1-per-iniziare)
2. [Tutorial: la tua prima sessione di loop](#2-tutorial-la-tua-prima-sessione-di-loop)
3. [Descrizione del pannello](#3-descrizione-del-pannello)
4. [Le tracce in dettaglio](#4-le-tracce-in-dettaglio)
5. [Sincronizzazione, quantizzazione e tempo](#5-sincronizzazione-quantizzazione-e-tempo)
6. [Drum machine](#6-drum-machine)
7. [Effetti](#7-effetti)
8. [Menu del display](#8-menu-del-display)
9. [Importazione ed esportazione](#9-importazione-ed-esportazione)
10. [Scorciatoie da tastiera](#10-scorciatoie-da-tastiera)
11. [Latenza e configurazione audio](#11-latenza-e-configurazione-audio)
12. [Risoluzione dei problemi](#12-risoluzione-dei-problemi)
13. [Note tecniche](#13-note-tecniche)

---

## 1. Per iniziare

### 1.1 Requisiti

a) Un browser desktop: Chrome, Edge o Firefox (versioni recenti). Safari potrebbe funzionare ma non è testato.

b) Un ingresso audio: un microfono integrato o USB, oppure un'interfaccia audio con chitarra, synth o microfono collegati.

c) **Cuffie**, fortemente consigliate quando registri da un microfono. Altrimenti il suono degli altoparlanti rientra nei loop.

### 1.2 Aprire il looper

a) **Online:** apri la [versione live](https://droogia.github.io/loop-gizmo/).

b) **Offline:** scarica `index.html` dal repository e fai doppio clic. È tutto in quel file: nessuna installazione e nessuna connessione Internet necessaria.

### 1.3 Accensione

All'apertura la pagina mostra la schermata **⏻ POWER ON**. I browser permettono l'audio solo dopo un clic dell'utente, ed è questo il clic.

a) Fai clic su **POWER ON**.

b) Il browser chiede l'accesso al microfono: consentilo. Se hai più ingressi (per esempio un'interfaccia audio), il browser usa quello predefinito. Per sceglierne un altro, cambialo nelle impostazioni del sito (l'icona accanto alla barra degli indirizzi), poi usa **MENU → MICROPHONE** per ricollegarlo.

c) Se l'ingresso funziona, il display mostra `MIC: <nome dispositivo>`; se l'accesso è stato negato, mostra `MIC N/A`. Senza microfono puoi comunque usare la drum machine e caricare file audio sulle tracce.

### 1.4 Controllare il livello d'ingresso

a) Emetti un suono: l'indicatore **IN** sul display si muove.

b) Regola la terza manopola centrale, **IN.LV**, in modo che le note forti riempiano quasi tutto l'indicatore senza restare fisse al massimo.

c) Per ascoltare l'ingresso dal vivo attraverso il looper, attiva **MENU → INPUT MONITOR**. Lascialo spento se la tua interfaccia ha già il monitoraggio diretto.

---

## 2. Tutorial: la tua prima sessione di loop

Questo percorso costruisce un breve brano con batteria, linea di basso, accordi, melodia e una variazione d'effetto. Usa le scorciatoie da tastiera, ma ognuna corrisponde a un pulsante sullo schermo (vedi la sezione 10).

### Lezione 1 — Loop libero, senza batteria

a) Premi **`1`** (o fai clic sul pad grande della traccia 1). L'anello intorno al pad diventa **rosso** e lampeggia: stai registrando.

b) Suona una frase di qualche secondo: una sequenza di accordi, un ritmo battuto sul tavolo, qualsiasi cosa.

c) Premi di nuovo **`1`** esattamente nel punto in cui la frase deve ricominciare. L'anello diventa **giallo**: la traccia 1 ora ripete quello che hai registrato e sei in **sovraincisione** (overdub, cioè aggiungi sopra).

d) Suona un secondo strato sopra il loop.

e) Premi ancora **`1`**. L'anello diventa **verde**: semplice riproduzione, non si registra nulla.

f) Premi **`Q`** (o il pulsante ■ STOP della traccia 1) per fermare la traccia. Premi **`1`** per farla ripartire.

> La lunghezza di questo primo loop è ora il **loop master**. Il tempo mostrato sul display è stato calcolato da esso, e ogni traccia successiva si allinea a lui.

### Lezione 2 — Annulla e ripristina

a) Con la traccia 1 in riproduzione, premi **`1`** per sovraincidere e aggiungi qualcosa che non ti piace.

b) Premi **`Z`** (UNDO/REDO): l'ultimo passaggio di sovraincisione sparisce.

c) Premi di nuovo **`Z`** per ripristinarlo (redo). Una terza pressione lo toglie di nuovo.

L'annullamento agisce sull'**ultima traccia registrata o sovraincisa** e ricorda un solo passaggio. Il pulsante UNDO/REDO si illumina quando c'è qualcosa da annullare o ripristinare.

### Lezione 3 — Cancellare

Tieni premuto **`Q`** (o il pulsante ■ della traccia 1) per un secondo. Il display mostra `TRACK 1 CLEARED`. Quando tutte le tracce sono vuote, il loop master si azzera e la registrazione successiva stabilisce una nuova lunghezza.

### Lezione 4 — Partire dalla batteria

a) Premi qualche volta **RHYTHM EDIT** per scegliere un pattern. Il nome compare in alto a destra sul display.

b) Imposta il tempo: gira la prima manopola centrale (**TEMPO**), oppure batti **`G`** (TAP TEMPO) quattro volte a tempo. Il pulsante TAP TEMPO lampeggia a ogni battito.

c) Premi **`B`** (RHYTHM START/STOP). La batteria suona e il display conta `MEAS` (battuta) e `BEAT` (movimento).

d) Regola il volume della batteria con la seconda manopola centrale (**RHY.LV**).

Mentre la batteria suona, **una battuta del ritmo è il loop master**, e ogni registrazione dura un numero intero di battute.

### Lezione 5 — Costruire un brano a strati

Con la batteria in funzione:

a) **Basso sulla traccia 1:** premi **`1`** poco prima dell'inizio di una battuta. Con **REC QUANTIZE** impostato su MEASURE (il valore predefinito), l'anello lampeggia in **arancione (WAIT)** e la registrazione parte esattamente sul battere successivo. Suona due battute di basso.

b) Premi **`1`** verso la fine della seconda battuta. La registrazione prosegue fino alla stanghetta e poi passa a sovraincisione/riproduzione. Che tu prema un po' prima o un po' dopo, il loop si aggancia a battute intere.

c) Premi ancora **`1`** se vuoi la semplice riproduzione.

d) **Accordi sulla traccia 2:** premi **`2`** e suona quattro battute. La traccia 2 può essere più lunga della traccia 1: le tracce restano in fase, e la traccia 1 semplicemente si ripete due volte sotto la traccia 2.

e) **Melodia sulla traccia 3:** premi **`3`**, suona, e premi **`3`** per chiudere il loop.

f) **Mix:** usa il **fader** di ogni traccia per il volume. Per collocarla nel panorama stereo, fai clic su **TRACK** nella striscia e gira la quarta manopola centrale (**PAN**).

### Lezione 6 — Suonare con gli effetti

a) Fai clic sul pulsante **FX** della traccia 2 in modo che si illumini. La traccia 2 ora passa attraverso i Track FX.

b) Scegli il banco **A** a destra (TRACK FX). Per impostazione predefinita è **FILTER**.

c) Gira lentamente la manopola grande **TRACK FX** avanti e indietro: gli accordi passano da ovattati ad aperti.

d) Premi **EDIT** sopra di essa per cambiare il tipo del banco A. Prova **FLANGER**, poi **WAH-WAH**. Con WAH-WAH la manopola grande funziona come il pedale: muovila avanti e indietro.

e) Ora un **effetto d'ingresso**: fai clic su **C** a sinistra (INPUT FX) e premi l'**EDIT** di sinistra finché compare **TRANSPOSE**. Imposta la manopola grande di sinistra su **−12 st**. Tutto ciò che suoni è ora un'ottava più basso: puoi registrare una linea di basso un'ottava sotto con una chitarra. Fai di nuovo clic su **C** per spegnere l'effetto d'ingresso.

### Lezione 7 — Arrangiamento e finale

a) **Breakdown:** premi **`W`** ed **`E`** per fermare le tracce 2 e 3, lasciando batteria e basso.

b) **Ripresa:** premi **`2`** e **`3`** per farle rientrare. Rientrano in fase.

c) **Effetto reverse:** fai clic su **TRACK** della traccia 3, seleziona **REVERSE** con ◀ ▶ e premi **ENTER**. La melodia suona al contrario. Premi **EXIT** per uscire dalla pagina.

d) **Finale:** premi **Spazio** (ALL START/STOP). Tutte le tracce e la batteria si fermano insieme. Premi di nuovo **Spazio** per far ripartire tutto dall'inizio del loop.

e) **Salva il lavoro:** per ogni traccia, fai clic su **TRACK → EXPORT WAV** per salvare un file `.wav`.

Hai usato tutte le funzioni principali. Le sezioni seguenti descrivono ogni comando nel dettaglio.

---

## 3. Descrizione del pannello

### 3.1 Sezione superiore

| Comando | Funzione |
|---|---|
| **Manopola grande INPUT FX** (sinistra) | Quantità (oppure semitoni / posizione del pedale) del banco di effetti d'ingresso selezionato |
| **INPUT FX EDIT** | Cambia ciclicamente il tipo di effetto del banco d'ingresso selezionato |
| **MENU** | Apre/chiude la pagina SYSTEM MENU sul display |
| **LOOP** | Apre/chiude la pagina LOOP SETTINGS |
| **Display (LCD)** | Stato e menu (sezione 8) |
| **EXIT ✕** | Torna alla pagina principale del display |
| **ENTER ●** | Modifica la voce di menu selezionata; nella pagina principale apre la pagina della traccia selezionata |
| **◀ ▶** | Nella pagina principale: seleziona la traccia precedente/successiva. Nei menu: sposta il cursore |
| **OUTPUT LEVEL** | Volume generale |
| **RHYTHM EDIT** | Pattern ritmico successivo |
| **TRACK FX EDIT** | Cambia ciclicamente il tipo di effetto del banco di traccia selezionato |
| **Manopola grande TRACK FX** (destra) | Quantità del banco di effetti di traccia selezionato |

### 3.2 Fila centrale

| Comando | Funzione |
|---|---|
| **INPUT FX A B C D** | Seleziona e accende un banco di effetti d'ingresso. Un nuovo clic sul banco acceso spegne gli effetti d'ingresso |
| **ALL START/STOP** | Ferma tutte le tracce e la batteria; premuto di nuovo, fa ripartire dall'inizio ogni traccia con contenuto (e la batteria, se era in funzione) |
| **UNDO/REDO** | Annulla l'ultimo passaggio di registrazione/sovraincisione; premuto di nuovo, lo ripristina |
| **Manopola TEMPO** | Tempo della batteria (40–250 BPM). Bloccato quando esiste un loop |
| **Manopola RHY.LV** | Volume della batteria |
| **Manopola IN.LV** | Guadagno d'ingresso (prima degli effetti d'ingresso) |
| **Manopola PAN** | Panorama della traccia selezionata (indicata come `PAN n`) |
| **TAP TEMPO** | Batti almeno due volte per impostare il tempo; lampeggia a ogni battito |
| **RHYTHM START/STOP** | Avvia/ferma la batteria |
| **TRACK FX A B C D** | Sceglie il banco di effetti attivo per tutte le tracce che hanno il pulsante FX acceso |

### 3.3 Strisce delle tracce (1–6)

| Comando | Funzione |
|---|---|
| **FX** | Fa passare la traccia attraverso il banco Track FX attivo |
| **TRACK** | Seleziona la traccia e apre la sua pagina di impostazioni sul display |
| **■ STOP** | Ferma la traccia. **Tenuto premuto 1 s la cancella** |
| **Fader** | Volume di riproduzione della traccia |
| **Indicatore di lunghezza** | Durata del loop in secondi e in battute |
| **Pad grande** | Registra / sovraincidi / riproduci (vedi 4.1) |
| **Anello** | Mostra lo stato e la posizione nel loop (vedi 4.2) |

Tutte le manopole e i fader rispondono al **trascinamento verticale** e alla **rotella del mouse**. Tieni premuto **Maiusc** mentre trascini una manopola per una regolazione fine. Un **doppio clic** riporta manopola o fader al valore predefinito.

---

## 4. Le tracce in dettaglio

### 4.1 Cosa fa il pad grande

L'effetto di una pressione dipende dallo stato attuale della traccia e da **REC ACTION** (pagina LOOP).

| Stato attuale | REC→DUB→PLAY (predefinito) | REC→PLAY→DUB |
|---|---|---|
| Vuota | Avvia la registrazione | Avvia la registrazione |
| In registrazione | Chiude il loop → **sovraincisione** | Chiude il loop → **riproduzione** |
| In sovraincisione | → Riproduzione | → Riproduzione |
| In riproduzione | → Sovraincisione | → Sovraincisione |
| Ferma | → Riproduzione | → Riproduzione |

Una traccia **one-shot** (vedi 4.4) si comporta diversamente: ogni pressione la fa ripartire dall'inizio e non sovraincide.

### 4.2 Colori dell'anello

| Anello | Significato |
|---|---|
| Scuro | Vuota |
| **Rosso**, lampeggiante | Registrazione del primo loop (lunghezza libera) |
| **Rosso**, che si riempie | Registrazione sincronizzata al loop master |
| **Arancione**, lampeggiante | WAIT: la registrazione parte alla prossima stanghetta |
| **Giallo**, che si riempie | Sovraincisione |
| **Verde**, che si riempie | Riproduzione; l'arco pieno indica la posizione nel loop |
| Grigio | Ferma (contiene ancora audio) |

Il testo sotto il pad ripete lo stato. Durante una registrazione sincronizzata che hai già chiuso, indica cosa succede dopo (per esempio `REC → DUB`).

### 4.3 Sovraincisione

La sovraincisione aggiunge nuovo audio sopra il loop esistente. La lunghezza del loop non cambia mai durante una sovraincisione. Ogni passaggio di sovraincisione (dall'ingresso in DUB all'uscita) è un singolo passo di annullamento.

### 4.4 Impostazioni della traccia (pagina TRACK)

| Voce | Valori | Effetto |
|---|---|---|
| REVERSE | ON / OFF | Riproduce il loop al contrario. Anche le sovraincisioni su una traccia invertita vengono scritte al contrario, così restano allineate a ciò che senti |
| ONE SHOT | ON / OFF | A ogni pressione del pad la traccia suona una volta dall'inizio, poi si ferma. Utile per campioni ed effetti singoli |
| TRACK FX | ON / OFF | Uguale al pulsante FX della striscia |
| PAN | L50 … C … R50 | Uguale alla manopola PAN. ENTER / clic scorre i valori |
| IMPORT AUDIO… | — | Carica un file audio su questa traccia (sezione 9) |
| EXPORT WAV | — | Salva questa traccia come WAV stereo a 16 bit (sezione 9) |

### 4.5 Fermare e cancellare

a) **Stop:** breve pressione su ■ (o `Q` `W` `E` `R` `T` `Y`). Se la traccia sta registrando, prima il loop si chiude e poi la traccia si ferma.

b) **Cancellazione:** tieni premuto ■ per 1 secondo. Questo elimina anche la memoria di annullamento/ripristino della traccia.

c) Quando tutte le tracce sono cancellate (e la batteria è spenta), il loop master si azzera.

---

## 5. Sincronizzazione, quantizzazione e tempo

### 5.1 Il loop master

Tutte le tracce condividono un'unica linea temporale, il **loop master**, che si stabilisce in uno di due modi:

a) **Con la prima registrazione**, se la batteria non è in funzione. La frase che registri definisce la lunghezza master, e il tempo si ricava presumendo che il loop contenga un numero intero di battute in 4/4. Il looper sceglie il numero di battute che porta il tempo ad almeno 75 BPM: un loop di 2 secondi diventa 1 battuta a 120 BPM, uno di 6 secondi diventa 2 battute a 80 BPM.

b) **Con la batteria**, se la avvii prima di registrare qualcosa. Il master è allora una battuta al tempo corrente.

La pagina LOOP mostra la lunghezza master in secondi e battute (`LOOP LENGTH`).

### 5.2 Registrazione sincronizzata

Quando esiste un loop master, ogni nuova registrazione:

a) **Inizia** su una stanghetta (l'inizio del loop master), se REC QUANTIZE è su MEASURE. Se premi durante circa il primo 12% del loop, la registrazione parte subito dall'inizio di quel loop, così una pressione leggermente in ritardo prende comunque il battere. Altrimenti la traccia attende (arancione) l'inizio del loop successivo.

b) **Termina** su un multiplo intero della lunghezza master. Una pressione entro circa il primo 12% di un nuovo ciclo arrotonda per difetto; una pressione più tarda arrotonda per eccesso, e la registrazione continua fino al confine successivo.

Con REC QUANTIZE su **OFF** la registrazione parte subito. La parte del loop prima della pressione resta muta, e la fine viene comunque arrotondata a un multiplo intero.

### 5.3 Fase

Le tracce non vanno mai fuori sincrono: ognuna suona sempre la parte del proprio loop che corrisponde alla linea temporale comune. Una traccia lunga il doppio del master suona la prima metà e poi la seconda, mentre una traccia lunga quanto il master si ripete due volte.

### 5.4 Ripartire dall'inizio

Quando non suona nulla (tutte le tracce ferme, batteria spenta), il successivo avvio (una singola traccia, ALL START o la batteria) **riazzera la linea temporale**, e la riproduzione parte dall'inizio del loop.

### 5.5 Tempo

a) Il tempo si può cambiare solo quando **non esiste alcun loop**. Dopo, il display mostra `TEMPO LOCKED`, perché cambiare il tempo cambierebbe la lunghezza dei loop.

b) TAP TEMPO calcola la media dei colpi battuti a meno di 2,5 secondi l'uno dall'altro.

c) Gli effetti DELAY e FLANGER seguono il tempo: il delay ripete su una croma puntata e il flanger compie una spazzata ogni due battute.

---

## 6. Drum machine

### 6.1 Pattern

| Pattern | Descrizione |
|---|---|
| ROCK | Hi-hat in crome dritte, cassa sull'1, sul 3 e sul "e" del 3 |
| POP | Hi-hat in semicrome, cassa sincopata |
| FUNK | Cassa movimentata e ghost note di rullante, hi-hat aperto |
| SHUFFLE | Crome swing (sensazione di terzina) |
| HIPHOP | Cassa rilassata con un leggero swing |
| 4 FLOOR | Cassa su ogni movimento, hi-hat aperto in levare |
| METRO | Clic di metronomo, accentato sul primo movimento di ogni loop |

Premi **RHYTHM EDIT**, oppure usa **MENU → RHYTHM PATTERN**, per cambiare pattern. Il cambio è immediato, anche mentre la batteria suona.

### 6.2 Come la batteria segue i loop

La batteria è agganciata al loop master. Se la avvii mentre le tracce suonano, entra a tempo. Se il primo loop è stato registrato liberamente, la batteria usa il tempo e il numero di battute ricavati da esso (5.1).

I suoni di batteria sono sintetizzati in tempo reale (cassa, rullante, hi-hat chiuso e aperto, clic), quindi non ci sono campioni da caricare.

---

## 7. Effetti

### 7.1 Input FX e Track FX

a) Gli **Input FX** elaborano ciò che suoni **prima che venga registrato**: l'effetto diventa parte del loop. Esempio: registra una linea di basso attraverso TRANSPOSE −12.

b) I **Track FX** elaborano la **riproduzione** di una traccia. La registrazione resta pulita, e puoi cambiare o togliere l'effetto in qualsiasi momento. Ogni traccia li attiva con il proprio pulsante **FX**, e tutte le tracce attivate usano il banco attivo (A–D).

Ogni sezione ha quattro banchi. Ogni banco contiene un tipo di effetto, che si cambia con **EDIT**, e una propria regolazione della manopola.

Banchi predefiniti:

| Banco | Input FX | Track FX |
|---|---|---|
| A | REVERB | FILTER |
| B | DELAY | DELAY |
| C | RING MOD | REVERB |
| D | LO-FI | LO-FI |

### 7.2 Tipi di effetto

| Tipo | Cosa controlla la manopola grande | Note |
|---|---|---|
| **FILTER** | Frequenza di taglio di un passa-basso risonante: tutto a sinistra = aperto, tutto a destra = chiuso | Classica spazzata da DJ |
| **DELAY** | Livello dell'effetto e numero di ripetizioni | Croma puntata sincronizzata al tempo, ripetizioni scurite |
| **REVERB** | Quantità di riverbero | Sala di circa 2,4 s |
| **LO-FI** | Risoluzione in bit (da 16 a 3 bit) e banda passante | Da leggermente sporco a fortemente degradato |
| **RING MOD** | Frequenza della portante (30–930 Hz) | Timbri metallici o robotici |
| **FLANGER** | Intensità (profondità, feedback, miscela) | Spazzata "a jet" su 2 battute |
| **WAH-WAH** | **Posizione del pedale**: sinistra = tallone (scuro), destra = punta (brillante) | Muovi la manopola come un pedale |
| **TRANSPOSE** | Intonazione in semitoni, −12 … +12 (centro = 0) | Cambio d'intonazione che mantiene la durata; doppio clic sulla manopola per tornare a 0 |

Il valore sotto ogni manopola grande mostra la regolazione nell'unità propria dell'effetto: `%`, `PEDAL %` oppure `±n st`.

### 7.3 Suggerimenti

a) **Strati d'ottava:** registra una parte, poi sovraincidila di nuovo con TRANSPOSE +12 sull'ingresso, per un effetto chitarra a 12 corde o organo.

b) **Spazzate di wah:** imposta un banco Track FX su WAH-WAH e muovi la manopola a tempo con il ritmo.

c) **Breakdown:** metti FILTER su tutte le tracce (FX acceso), abbassa gradualmente la frequenza di taglio per quattro battute e riaprila di colpo sul drop.

d) **Reverse + riverbero:** imposta REVERSE su una traccia e aggiungi REVERB dai Track FX per crescendo spettrali.

---

## 8. Menu del display

### 8.1 Pagina principale

```
MEMORY 01          ♩=120.0          ROCK ▶
[1 P][2 D][3  ][4  ][5  ][6 S]          ← stato delle tracce (R/D/P/S/W)
[■■■■■■■■■■■■·········]                 ← posizione nel loop master
MEAS 01/02  BEAT 3            IFX:REVERB
IN ▮▮▮   OUT ▮▮▮▮▮           MIC: ...
TEMPO   RHY.LV 60   IN.LV 80   PAN1 C   ← etichette delle manopole centrali
```

Le caselle evidenziate indicano le tracce attive. Se la traccia selezionata è vuota, anche la sua casella è evidenziata.

### 8.2 Navigazione

a) **◀ ▶** o i **tasti freccia** spostano il cursore.

b) **ENTER** porta la voce selezionata al valore successivo.

c) **Clic** su una voce per il valore successivo; **clic destro** o **Maiusc+clic** per il valore precedente. Anche la **rotella del mouse** sopra una voce la modifica.

d) **EXIT** o **Esc** tornano alla pagina principale.

### 8.3 LOOP SETTINGS (pulsante LOOP)

| Voce | Valori |
|---|---|
| REC ACTION | REC→DUB→PLAY / REC→PLAY→DUB |
| REC QUANTIZE | MEASURE / OFF |
| LATENCY COMP | AUTO, oppure 0 … 100 ms |
| LOOP LENGTH | Lunghezza master (solo visualizzazione) |

### 8.4 SYSTEM MENU (pulsante MENU)

| Voce | Valori |
|---|---|
| INPUT MONITOR | ON / OFF: ascolto dell'ingresso dal vivo |
| MICROPHONE | Mostra il dispositivo; ENTER lo scollega o lo ricollega |
| RHYTHM PATTERN | Elenco dei pattern |
| RHYTHM TEMPO | ENTER / clic aggiunge 1 BPM, clic destro lo toglie |

### 8.5 Pagina TRACK (pulsante TRACK)

Vedi 4.4.

---

## 9. Importazione ed esportazione

### 9.1 Importare audio

Trascina un file audio (WAV, MP3, OGG, FLAC, M4A: qualsiasi formato che il browser sappia decodificare) **su una striscia di traccia**, oppure usa **TRACK → IMPORT AUDIO…**.

a) Se non esiste un loop master, la durata del file diventa il loop master.

b) Se esiste un loop master, il file viene allungato con silenzio o accorciato al multiplo intero più vicino.

c) La traccia resta **ferma**: premi il suo pad per riprodurla.

d) L'importazione si può annullare con UNDO.

### 9.2 Esportare

**TRACK → EXPORT WAV** salva la traccia selezionata come `loop-gizmo-trackN.wav` (stereo a 16 bit, alla frequenza di campionamento del browser). Se REVERSE è attivo, anche il file esportato è invertito. Track FX, fader e panorama **non** sono inclusi nell'esportazione.

> I loop sono conservati solo nella memoria del browser. **Ricaricare o chiudere la pagina li cancella.** Esporta tutto ciò che vuoi conservare.

---

## 10. Scorciatoie da tastiera

| Tasto | Azione | Equivalente sullo schermo |
|---|---|---|
| `1` … `6` | Registra / sovraincidi / riproduci la traccia 1–6 | Pad grande |
| `Q` `W` `E` `R` `T` `Y` | Ferma la traccia 1–6; tenuto 1 s la cancella | Pulsante ■ |
| `Spazio` | Avvio/arresto generale | ALL START/STOP |
| `Z` | Annulla / ripristina | UNDO/REDO |
| `B` | Avvio/arresto della batteria | RHYTHM START/STOP |
| `G` | Tap tempo | TAP TEMPO |
| `←` `→` `↑` `↓` | Selezione traccia / cursore dei menu | ◀ ▶ |
| `Invio` | Enter | ENTER |
| `Esc` | Torna alla pagina principale | EXIT |

Le scorciatoie vengono ignorate se è premuto Ctrl, Alt o Cmd, così le scorciatoie del browser continuano a funzionare.

---

## 11. Latenza e configurazione audio

### 11.1 Perché le sovraincisioni possono risultare in ritardo

Il suono impiega un certo tempo per arrivare dal looper alle tue orecchie (latenza d'uscita) e dallo strumento al looper (latenza d'ingresso). Quando suoni insieme a un loop, quindi, ciò che registri arriva leggermente in ritardo. **LATENCY COMP** anticipa le sovraincisioni e le registrazioni sincronizzate di quella quantità.

a) **AUTO** usa la latenza dichiarata dal browser più un piccolo margine. Il valore in uso è mostrato accanto.

b) Se le sovraincisioni suonano ancora in ritardo (con un effetto di "flam"), scegli un valore fisso più alto. Se suonano in anticipo, scegline uno più basso.

c) **Suggerimento per la calibrazione:** avvia il pattern METRO, registra su una traccia dei battiti di mani esattamente sui clic e riascoltala con la batteria. Regola LATENCY COMP finché battiti e clic suonano come un unico suono.

### 11.2 Ridurre la latenza

a) **Windows:** usa Chrome o Edge con l'interfaccia audio impostata come dispositivo predefinito, con un buffer basso nel suo pannello di controllo. Chiudi le altre applicazioni che usano molto l'audio.

b) Le cuffie Bluetooth aggiungono molta latenza (spesso 150 ms o più). Per registrare usa cuffie con il filo.

### 11.3 Ingresso pulito

Il looper chiede al browser di disattivare cancellazione dell'eco, soppressione del rumore e controllo automatico del guadagno. Sono funzioni pensate per le chiamate vocali e peggiorano la musica.

---

## 12. Risoluzione dei problemi

| Problema | Soluzione |
|---|---|
| `MIC N/A` sul display | Consenti l'accesso al microfono per la pagina (l'icona accanto alla barra degli indirizzi), poi **MENU → MICROPHONE → ENTER** |
| Dispositivo d'ingresso sbagliato | Cambia il microfono del sito nelle impostazioni del browser, poi ricollegalo con **MENU → MICROPHONE** |
| Fischio di feedback (Larsen) | Usa le cuffie, oppure spegni **INPUT MONITOR** |
| Senti l'ingresso due volte | Spegni INPUT MONITOR se la tua interfaccia ha già il monitoraggio diretto |
| Sovraincisioni fuori tempo | Regola **LATENCY COMP** (11.1) |
| `TEMPO LOCKED` | Il tempo cambia solo quando non esiste alcun loop. Cancella tutte le tracce (e ferma la batteria, se il master viene da un loop registrato) |
| La registrazione non è partita | Probabilmente l'anello lampeggia in arancione (WAIT): partirà alla prossima stanghetta. Disattiva REC QUANTIZE per una partenza immediata |
| Un'interruzione del suono all'inizio di una sovraincisione su un loop molto lungo | In quel momento viene fatta la copia per l'annullamento. Tieni i loop sotto il minuto circa, o sovraincidi meno spesso |
| Nessun suono | Controlla OUTPUT LEVEL e i fader delle tracce, e assicurati di aver premuto POWER ON |
| "Audio engine failed" | Usa una versione aggiornata di Chrome, Edge o Firefox |

---

## 13. Note tecniche

a) **Motore:** un processore AudioWorklet dedicato gestisce tutte e sei le tracce con precisione al singolo campione. Registrazione, sovraincisione, avvii e chiusure quantizzati e copie per l'annullamento avvengono tutti nel thread audio. Ogni traccia ha la propria uscita stereo, instradata attraverso l'inserto FX, il fader, il pan e il limiter generale.

b) **TRANSPOSE:** un secondo processore AudioWorklet che esegue un pitch shifting granulare, con due testine di lettura sovrapposte in dissolvenza incrociata tramite finestre a potenza complementare (grani da 60 ms).

c) **Memoria:** ogni secondo di audio stereo occupa circa 0,4 MB per traccia a 48 kHz, più una copia per l'annullamento per traccia.

d) **File unico:** tutto il codice, gli stili e i suoni sono dentro `index.html`. Nulla viene caricato dalla rete.

---

*Loop Gizmo è un progetto indipendente e non è affiliato ad alcun produttore di hardware.*
