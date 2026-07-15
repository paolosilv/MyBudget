# 🚀 MyBudget — Roadmap

## Visione del prodotto

MyBudget è un'applicazione progettata per trasformare semplici movimenti
economici in informazioni chiare, immediate e utili.

Il suo scopo non è soltanto registrare entrate e uscite, ma aiutare l'utente a:

- comprendere la propria situazione economica;
- controllare l'andamento del proprio budget;
- confrontare periodi diversi;
- individuare abitudini e variazioni;
- prendere decisioni più consapevoli;
- verificare nel tempo gli effetti delle proprie decisioni.

Le informazioni più importanti devono essere disponibili immediatamente,
senza richiedere calcoli manuali o ricerche tra note, documenti e movimenti.

---

## Principio guida

La schermata iniziale deve permettere all'utente di comprendere
la propria situazione economica mensile entro pochi secondi.

L'informazione principale sarà:

> Il bilancio attuale del mese.

Intorno a questo dato verranno progressivamente aggiunti:

- totale delle entrate;
- totale delle uscite;
- percentuale del budget ordinario utilizzato;
- percentuale del budget per spese extra utilizzato;
- budget residuo;
- confronto con il mese precedente;
- previsione di fine mese;
- suggerimenti diretti;
- avvisi e informazioni rilevanti.

---

## Ciclo di MyBudget

MyBudget seguirà un processo ciclico composto da sei fasi.

### 1. Configura

L'utente definisce la propria situazione economica iniziale,
i budget e gli obiettivi personali.

### 2. Registra

L'utente inserisce rapidamente entrate e uscite.

### 3. Osserva

L'app trasforma i movimenti registrati in una panoramica chiara.

### 4. Comprende

MyBudget evidenzia tendenze, confronti, anomalie e informazioni utili.

### 5. Decide

L'utente prende decisioni sulla base delle informazioni ricevute.

### 6. Verifica

Nei periodi successivi l'utente controlla gli effetti delle proprie decisioni.

---

## Dashboard futura

La dashboard completa dovrà mostrare una panoramica simile alla seguente:

```text
MYBUDGET

Bilancio del mese
+ 650 €

Entrate
2.100 €

Uscite
1.450 €

Budget ordinario utilizzato
72%

Budget spese extra utilizzato
35%

Confronto con il mese precedente
+ 220 €

Consiglio rapido
"Se mantieni questo ritmo, terminerai il mese
con circa 500 € disponibili."
```

Dalla dashboard sarà possibile accedere alle seguenti sezioni:

- movimenti del mese corrente;
- dettaglio delle entrate;
- dettaglio delle uscite;
- categorie di spesa;
- metodi di pagamento;
- budget ordinario;
- budget per spese extra;
- statistiche del mese;
- confronto con i mesi precedenti;
- panoramica annuale;
- obiettivi economici;
- suggerimenti personalizzati;
- analisi basate sull'Intelligenza Artificiale.

Questa sezione descrive la direzione finale del prodotto.

Le funzionalità verranno implementate gradualmente,
senza tentare di costruire tutto nelle prime versioni.

---

# Versioni del progetto

## v0.0 — Preparazione del progetto

### Obiettivo

Preparare l'ambiente di lavoro e organizzare correttamente il progetto.

### Attività

- [x] Scelta del nome `MyBudget`
- [x] Creazione della cartella locale
- [x] Creazione del file `README.md`
- [x] Creazione del file `ROADMAP.md`
- [x] Creazione del file `PROGRESS.md`
- [ ] Creazione del repository GitHub
- [ ] Scelta dello stack tecnologico iniziale
- [ ] Creazione del progetto applicativo
- [ ] Apertura del progetto nell'ambiente di sviluppo
- [ ] Primo avvio locale
- [ ] Primo commit Git

### Risultato atteso

Un progetto vuoto, organizzato, documentato, versionato e avviabile in locale.

---

## v0.1 — Bilancio essenziale

### Obiettivo

Realizzare la prima versione realmente utilizzabile di MyBudget.

L'utente deve poter registrare entrate e uscite
e comprendere immediatamente il proprio bilancio mensile.

### Funzionalità

- [ ] Impostazione del saldo iniziale
- [ ] Inserimento di un movimento
- [ ] Selezione del tipo: `ENTRATA` oppure `USCITA`
- [ ] Inserimento dell'importo
- [ ] Inserimento di una descrizione
- [ ] Registrazione automatica della data
- [ ] Salvataggio permanente dei movimenti
- [ ] Visualizzazione della lista dei movimenti
- [ ] Calcolo delle entrate del mese corrente
- [ ] Calcolo delle uscite del mese corrente
- [ ] Calcolo del bilancio del mese corrente
- [ ] Visualizzazione del bilancio del mese precedente, se disponibile

### Schermata prevista

```text
MYBUDGET

Bilancio luglio
+ 650 €

Entrate
2.100 €

Uscite
1.450 €

Mese precedente
+ 430 €

[ Aggiungi movimento ]

Ultimi movimenti

- Supermercato        -45 €
+ Stipendio         +2.100 €
- Palestra            -35 €
```

### Risultato atteso

MyBudget sostituisce le Note dell'iPhone
per la registrazione dei movimenti e per il calcolo manuale
del bilancio mensile.

---

## v0.2 — Gestione completa dei movimenti

### Obiettivo

Rendere più completa e ordinata la gestione di entrate e uscite.

### Funzionalità

- [ ] Modifica di un movimento
- [ ] Eliminazione di un movimento
- [ ] Conferma prima dell'eliminazione
- [ ] Categorie delle entrate e delle uscite
- [ ] Metodo di pagamento
- [ ] Filtri per tipo
- [ ] Filtri per categoria
- [ ] Filtri per intervallo di date
- [ ] Ricerca nei movimenti
- [ ] Ordinamento dei movimenti

---

## v0.3 — Gestione del budget

### Obiettivo

Permettere all'utente di definire e controllare i propri limiti di spesa.

### Funzionalità

- [ ] Definizione del budget mensile ordinario
- [ ] Definizione del budget per spese extra
- [ ] Percentuale del budget ordinario utilizzato
- [ ] Percentuale del budget extra utilizzato
- [ ] Budget residuo
- [ ] Avvisi al raggiungimento di determinate soglie
- [ ] Evidenza del superamento del budget
- [ ] Budget differenziato per categoria

---

## v0.4 — Statistiche e storico

### Obiettivo

Trasformare i movimenti economici in informazioni facilmente leggibili.

### Funzionalità

- [ ] Storico dei mesi precedenti
- [ ] Confronto tra mese corrente e mese precedente
- [ ] Confronto tra più mesi
- [ ] Riepilogo annuale
- [ ] Media mensile delle entrate
- [ ] Media mensile delle uscite
- [ ] Statistiche per categoria
- [ ] Andamento del saldo
- [ ] Grafici riepilogativi

---

## v0.5 — Dashboard evoluta

### Obiettivo

Mostrare immediatamente le informazioni più importanti.

### Funzionalità

- [ ] Bilancio del mese in evidenza
- [ ] Entrate e uscite del mese
- [ ] Percentuali dei budget
- [ ] Budget residuo
- [ ] Confronto con il mese precedente
- [ ] Ultimi movimenti
- [ ] Informazioni e avvisi rilevanti
- [ ] Collegamenti rapidi alle sezioni di dettaglio
- [ ] Layout personalizzabile

---

## v0.6 — Esperienza mobile

### Obiettivo

Rendere MyBudget semplice e veloce da utilizzare tramite iPhone.

### Funzionalità

- [ ] Interfaccia responsive
- [ ] Form ottimizzato per mobile
- [ ] Inserimento di un movimento in pochi secondi
- [ ] Visualizzazione chiara dei dati da mobile
- [ ] Test tramite Safari su iPhone
- [ ] Aggiunta dell'app alla schermata Home
- [ ] Configurazione come Progressive Web App
- [ ] Icona e schermata iniziale

---

## v0.7 — Pubblicazione online

### Obiettivo

Rendere MyBudget disponibile in modo stabile da qualsiasi dispositivo.

### Funzionalità

- [ ] Scelta del servizio di hosting
- [ ] Pubblicazione dell'applicazione
- [ ] Configurazione del database online
- [ ] Gestione sicura delle configurazioni
- [ ] Configurazione HTTPS
- [ ] Backup dei dati
- [ ] Verifica dell'accesso da iPhone
- [ ] Monitoraggio degli errori

---

## v1.0 — Prima versione completa

### Obiettivo

Rilasciare una versione stabile e realmente utilizzabile nel quotidiano.

### Requisiti

- [ ] Inserimento e gestione dei movimenti
- [ ] Bilancio mensile
- [ ] Entrate e uscite
- [ ] Storico dei mesi
- [ ] Budget ordinario ed extra
- [ ] Dashboard responsive
- [ ] Accesso stabile da iPhone
- [ ] Persistenza e protezione dei dati
- [ ] Esperienza d'uso semplice e veloce

---

# Visione futura

## Personalizzazione

### Obiettivo

Adattare l'esperienza e i suggerimenti alle esigenze specifiche dell'utente.

### Funzionalità

- [ ] Definizione degli obiettivi economici
- [ ] Preferenze sul livello di risparmio
- [ ] Priorità personali
- [ ] Categorie protette
- [ ] Spese considerate indispensabili
- [ ] Livello di rigidità dei consigli
- [ ] Suggerimenti coerenti con gli obiettivi
- [ ] Verifica periodica dei progressi
- [ ] Revisione degli obiettivi nel tempo

## Patrimonio mensile e riconciliazione

### Obiettivo

Permettere all'utente di registrare periodicamente (ipoteticamente il primo del mese) una fotografia reale
del proprio patrimonio disponibile e confrontarla con il valore teorico
calcolato attraverso i movimenti registrati in MyBudget.

Il patrimonio mensile rappresenta la somma dei saldi reali
di tutti gli strumenti economici configurati dall'utente.

### Possibili componenti del patrimonio

- [ ] Conto corrente
- [ ] Carte ricaricabili
- [ ] Contanti
- [ ] Conti digitali, come Revolut
- [ ] Altri strumenti configurabili dall'utente

### Flusso previsto

- [ ] L'utente configura i propri strumenti economici
- [ ] Il primo giorno del mese inserisce il saldo reale di ogni strumento
- [ ] MyBudget calcola il patrimonio mensile totale
- [ ] Durante il mese vengono registrate entrate e uscite
- [ ] MyBudget calcola il patrimonio teorico atteso
- [ ] Il mese successivo l'utente inserisce un nuovo patrimonio reale
- [ ] Il sistema confronta patrimonio teorico e patrimonio reale
- [ ] Il sistema evidenzia l'eventuale discrepanza
- [ ] L'utente può verificare la presenza di movimenti mancanti o errati

### Esempio

Patrimonio reale al 1° luglio
5.000 €

Bilancio registrato nel mese
+ 300 €

Patrimonio teorico al 1° agosto
5.300 €

Patrimonio reale al 1° agosto
5.275 €

Discrepanza
- 25 €

---

## Intelligenza Artificiale

### Obiettivo

Utilizzare l'AI per trasformare i dati economici
in indicazioni comprensibili e realmente utili.

L'AI non dovrà essere una funzionalità decorativa,
ma uno strumento di consapevolezza e supporto decisionale.

### Funzionalità

- [ ] Categorizzazione automatica dei movimenti
- [ ] Riepilogo mensile in linguaggio naturale
- [ ] Analisi delle abitudini di spesa
- [ ] Confronto automatico tra periodi
- [ ] Individuazione di anomalie
- [ ] Previsione del bilancio di fine mese
- [ ] Suggerimenti personalizzati
- [ ] Identificazione delle principali variazioni
- [ ] Chat con i propri dati economici

### Possibili domande rivolte all'AI

- Quanto ho speso al supermercato negli ultimi tre mesi?
- Qual è la categoria in cui sto spendendo di più?
- Sto rispettando il mio obiettivo di risparmio?
- Quali spese sono aumentate rispetto al mese precedente?
- Quanto potrei avere disponibile alla fine del mese?

---

## AWS e Cloud

### Obiettivo

Utilizzare MyBudget anche come laboratorio pratico
per imparare servizi cloud e prepararsi alle certificazioni AWS.

### Possibili evoluzioni

- [ ] Deploy dell'applicazione su AWS
- [ ] Database gestito nel cloud
- [ ] Autenticazione degli utenti
- [ ] Gestione sicura dei segreti
- [ ] Storage per documenti e ricevute
- [ ] Monitoraggio e logging
- [ ] Backup automatici
- [ ] Pipeline di deploy
- [ ] Dominio personale
- [ ] Utilizzo di servizi AWS per funzionalità AI

---

## Possibili evoluzioni successive

- [ ] Supporto multiutente
- [ ] Registrazione e autenticazione
- [ ] Gestione di più conti
- [ ] Gestione di carte e contanti
- [ ] Obiettivi di risparmio
- [ ] Entrate e spese ricorrenti
- [ ] Importazione di file
- [ ] Esportazione in CSV o Excel
- [ ] Caricamento delle ricevute
- [ ] Lettura automatica delle ricevute
- [ ] Notifiche
- [ ] Modalità famiglia o budget condiviso

---

# Regola di sviluppo

Prima di aggiungere una nuova funzionalità bisogna chiedersi:

> Questa funzionalità è necessaria per completare la versione corrente?

Se la risposta è no:

1. viene annotata nella roadmap;
2. non viene implementata immediatamente;
3. si continua a lavorare sull'obiettivo della versione corrente.

L'obiettivo è far crescere MyBudget gradualmente,
mantenendo ogni versione piccola, comprensibile e completabile.

---

# Regola personale di apprendimento

Ogni sessione deve avere un obiettivo piccolo e concreto,
completamente affrontabile in circa 10-30 minuti.

Il successo della sessione non dipende dalla quantità di codice prodotto,
ma dall'aver mantenuto l'appuntamento con il progetto
e dall'aver compreso almeno un piccolo elemento nuovo.

Principi:

- costanza prima dell'intensità;
- comprensione prima della velocità;
- progresso prima della perfezione;
- ChatGPT come tutor, non come sostituto;
- un solo micro-step alla volta;
- non saltare due sessioni consecutive.

---

### Stack tecnologico iniziale

- Frontend: React
- Backend: Java 21 con Spring Boot
- Framework: Spring Boot
- API: REST con JSON
- Build backend: Maven
- Database: PostgreSQL
- Persistenza: Spring Data JPA e Hibernate
- Versionamento: Git e GitHub
- Deploy futuro: AWS
- Funzionalità AI: versioni future