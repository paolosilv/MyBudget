# Progress


## 14/07/2026

- Fatto: creati e sistemati README.md e ROADMAP.md
- Imparato: differenza tra visione del prodotto, roadmap e avanzamento
- Prossimo passo: creare il repository GitHub

-----

## 15-16/07/2026

1.
- Fatto: inizializzato il repository Git locale (`git init`).
- Imparato: un repository Git nasce con una propria struttura (`.git`) e una configurazione locale distinta (personalizzabile) da quella globale.
- Prossimo passo: capire come Git inizia a tracciare realmente i file del progetto.

2.
- Fatto: aggiunto file alla stagin area (`git add`)
- Imparato: che git non salva semplicemente un file ma la "fotografia" dello stato del progetto (che sia di uno o più file)
- Prossimo passo: capire cosa è un commit

3.
- Fatto: configurata l'identità Git locale (`user.name` e `user.email`), creato il primo commit di MyBudget e analizzato il database a object di Git.
- Imparato: Git è un database di object immutabili collegati tramite hash. Un commit (che è a sua volta un object) punta al root tree (al riferimento), i tree rappresentano la struttura del progetto (per questo un commit ha la fotografia di tutto il progetto) e referenziano tree (cartelle) / blob (file, foglie del grafo di Git, sia lui che oggetto tree vengono "scritti" tramite "git add"), mentre i blob contengono esclusivamente il contenuto dei file. Git riutilizza gli object immutati e crea solo quelli necessari (efficienza di Git, cambio un blob cambierà il suo oggetto e quindi il suo hash ma anche quello del sub tree che lo contiene, sarà un nuovo oggetto con nuovo hash).
- Prossimo passo: comprendere branch e `HEAD`.

-----

## 21/07/2026

- Fatto: definito il primo Domain Model di MyBudget con Movimento, Wallet e RilevazioneSaldo; creato e committato `docs/DOMAIN_MODEL.md`.
- Fatto: rinominato il branch principale da `master` a `main`.
- Fatto: collegato il repository locale al repository GitHub tramite il remote `origin`.
- Fatto: pubblicati su GitHub i branch `main` e `feature-movement-model`, configurando i rispettivi upstream.
- Imparato: un branch locale e il relativo branch remoto sono riferimenti distinti; l'upstream permette a Git di sapere automaticamente dove eseguire `push` e `pull`.
- Imparato: Git Credential Manager gestisce l'autenticazione HTTPS e può conservare credenziali non più valide, che devono essere rimosse per forzare un nuovo accesso.
- Prossimo passo: progettare l'architettura iniziale di MyBudget prima di generare il backend e il frontend.
