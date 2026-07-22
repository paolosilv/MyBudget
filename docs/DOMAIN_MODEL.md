# Domain Model

## Scopo

Questo documento descrive i principali concetti del dominio di MyBudget, le loro relazioni e le regole fondamentali che l'applicazione deve garantire.

Il modello rappresenta esclusivamente il denaro amministrato dall'utente. Soggetti esterni, come datori di lavoro, negozi o ristoranti, non vengono modellati come entità del sistema.

---

# Concetti del dominio

## Movimento

Un Movimento rappresenta un'operazione economica registrata dall'utente.

Può descrivere:

- un'entrata di denaro in un Wallet;
- un'uscita di denaro da un Wallet;
- un trasferimento di denaro tra due Wallet.

### Esempi

- Accredito dello stipendio sul conto BCC.
- Cena pagata tramite Revolut.
- Trasferimento di denaro da BCC a Revolut.

### Attributi

| Attributo | Descrizione |
|-----------|-------------|
| data | Giorno in cui è avvenuta l'operazione. |
| importo | Quantità di denaro coinvolta. |
| tipo | ENTRATA, USCITA o TRASFERIMENTO. |
| descrizione | Breve descrizione del movimento. |
| origine | Wallet dal quale esce il denaro. |
| destinazione | Wallet nel quale entra il denaro. |

---

## Wallet

Un Wallet rappresenta un contenitore di denaro amministrato dall'utente.

Può rappresentare:

- un conto bancario;
- una carta;
- un conto digitale;
- denaro contante;
- altri contenitori assimilabili.

### Esempi

- BCC
- Revolut
- Carta ricaricabile
- Contanti

### Attributi

| Attributo | Descrizione |
|-----------|-------------|
| nome | Nome scelto dall'utente. |
| tipo | Tipologia del Wallet. |
| attivo | Indica se può essere utilizzato per nuovi movimenti. |

### Tipi previsti

- CONTO_BANCARIO
- CARTA
- CONTANTI
- ALTRO

> Il Wallet **non memorizza il saldo**. Il saldo viene sempre calcolato a partire dalle Rilevazioni del saldo e dai Movimenti registrati.

---

## Rilevazione del saldo

Una Rilevazione del saldo rappresenta il saldo reale presente in un Wallet in una determinata data.

Serve sia per definire il valore iniziale del Wallet sia per verificare periodicamente che tutti i movimenti siano stati registrati.

### Attributi

| Attributo | Descrizione |
|-----------|-------------|
| data | Giorno della rilevazione. |
| saldoRilevato | Saldo reale indicato dall'utente. |
| wallet | Wallet a cui appartiene la rilevazione. |

> La rilevazione mensile è consigliata, ma non obbligatoria.

---

# Relazioni

Un Wallet può essere origine di molti Movimenti.

Un Wallet può essere destinazione di molti Movimenti.

Un Wallet può avere molte Rilevazioni del saldo.

```text
Wallet
│
├── origine ───────────────► Movimento
│
├── destinazione ─────────► Movimento
│
└── 1 -------- N ─────────► RilevazioneSaldo
```

---

# Regole del dominio

## Movimento

- L'importo è sempre positivo.
- Un Movimento è sempre di tipo ENTRATA, USCITA oppure TRASFERIMENTO.

### ENTRATA

- origine non registrata (esterna al dominio);
- destinazione obbligatoria.

### USCITA

- origine obbligatoria;
- destinazione non registrata (esterna al dominio).

### TRASFERIMENTO

- origine obbligatoria;
- destinazione obbligatoria;
- origine e destinazione devono essere Wallet differenti;
- non rappresenta né un'entrata né un'uscita del patrimonio complessivo.

---

## Wallet

- Un Wallet non memorizza il proprio saldo.
- Il saldo viene sempre ricavato dalle Rilevazioni del saldo e dai Movimenti.
- Un Wallet già utilizzato non può essere eliminato.
- Un Wallet può essere rinominato o disattivato.

---

## Rilevazione del saldo

- Ogni Rilevazione appartiene ad un Wallet.
- Un Wallet può avere più Rilevazioni nel tempo.
- Per uno stesso Wallet non possono esistere due Rilevazioni nella stessa data.
- Una Rilevazione non modifica automaticamente i Movimenti.
- Lo scostamento tra saldo rilevato e saldo calcolato è sempre derivato.

---

# Dati derivati

I seguenti dati non vengono memorizzati direttamente, ma calcolati dal sistema:

- saldo del Wallet;
- saldo complessivo;
- saldo mensile;
- totale entrate;
- totale uscite;
- scostamento tra saldo rilevato e saldo calcolato.

---

# Evoluzioni previste

Le seguenti funzionalità non fanno ancora parte della prima versione del dominio:

- categorie dei Movimenti;
- classificazione automatica tramite IA;
- promemoria per la rilevazione mensile del saldo;
- statistiche avanzate;
- bilanci previsionali;
- gestione delle rettifiche.