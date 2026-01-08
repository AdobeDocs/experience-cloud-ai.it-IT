---
title: Panoramica abilità creazione agente percorso
description: Scopri come utilizzare l’abilità di creazione di Journey Agent per creare percorsi di marketing attraverso prompt in linguaggio naturale in Journey Optimizer.
solution: Journey Optimizer
product: journey optimizer
role: Admin,User,Developer
source-git-commit: 037d9864f72610f745b336acf0cf1192b7f21aa0
workflow-type: tm+mt
source-wordcount: '1068'
ht-degree: 1%

---


# Percorsi Create Agent: panoramica delle abilità e guida utente

## Panoramica

L’agente di creazione percorsi consente agli utenti di Journey Optimizer di creare e configurare percorsi di marketing utilizzando un’interfaccia in linguaggio naturale. Con l’agente di creazione del Percorso, i professionisti possono creare rapidamente i percorsi descrivendo i loro requisiti nei prompt conversazionali. L’agente semplifica la creazione del percorso, consentendo agli addetti al marketing di concentrarsi sulla strategia anziché sulla configurazione tecnica.

>[!AVAILABILITY]
>
>L’agente di creazione Percorso è disponibile per tutti i clienti che hanno accesso all’Assistente IA. Tuttavia, per utilizzare completamente le funzioni di agente di creazione del Percorso, sono necessarie le seguenti autorizzazioni:
>
>**Gestisci Percorsi**: questa autorizzazione consente di creare nuovi percorsi direttamente nell&#39;Assistente IA.
>
>**Visualizza eventi di Percorso, origini dati e azioni**: questa autorizzazione garantisce che l&#39;Assistente AI possa eseguire ricerche tramite eventi di Percorso e azioni personalizzate.
>
>**Visualizza segmenti**: questa autorizzazione garantisce che l&#39;Assistente AI possa eseguire ricerche di segmenti di pubblico durante la creazione di un Percorso.
>
>**Gestisci segmenti**: questa autorizzazione consente di creare nuovi tipi di pubblico direttamente nell&#39;Assistente IA.

## Casi d’uso

### Casi d’uso principali per l’agente di creazione del Percorso

Il Percorso Crea agente offre funzionalità che possono essere utilizzate per accelerare l’esecuzione del marketing:

1. **Creazione percorso attivata da eventi**

   - Creazione di percorsi che si attivano in base a eventi cliente specifici.
   - Progetta risposte automatizzate alle azioni dei clienti in tempo reale.
   - Creare flussi di comunicazione personalizzati in base al comportamento del cliente.

1. **Creazione di percorsi con targeting di pubblico**

   - Crea percorsi rivolti a segmenti di pubblico specifici.
   - Progettazione di sequenze di comunicazione in più fasi con tempistiche strategiche.

1. **Creazione percorso attivata da un evento business**

   - Creazione di percorsi che si attivano in base a un particolare evento di business e si rivolgono a un pubblico specifico (ad esempio, il prodotto torna in magazzino o cambia il punteggio di gioco)
   - Creare flussi di comunicazione personalizzati in base al comportamento del cliente.

1. **Creazione del percorso di qualificazione del pubblico**

   - Crea percorsi che si attivano quando i profili entrano o escono da una definizione di segmento di pubblico.
   - Creare flussi di comunicazione personalizzati in base al comportamento del cliente.

1. **Flussi percorso condizionale**

   - Crea rami decisionali in base agli attributi del cliente.
   - Progetta percorsi suddivisi in base alle preferenze del cliente.

Per ciascuno di questi casi d’uso, l’agente traduce i requisiti di linguaggio naturale in configurazioni di percorso strutturate.

## Competenze nel campo di applicazione e fuori campo di applicazione

### **Nell&#39;ambito**

Le seguenti funzionalità sono supportate dall&#39;agente di creazione Percorsi:

- **Creazione di un percorso in linguaggio naturale**: consente agli utenti di descrivere il flusso di percorso in linguaggio di conversazione.
- **percorsi basati su eventi e su pubblico**: supporta sia i tipi di percorso basati su attivatori che quelli pianificati, nonché la qualificazione di eventi di business e pubblico.
- **Logica condizionale**: gestisce le suddivisioni e le diramazioni delle decisioni in base agli attributi del cliente.
- **Messaggistica multicanale**: supporta notifiche push, e-mail e canali SMS.
- **Pianificazione Percorsi**: configura le date di inizio e gli orari per i percorsi pianificati.

### **Fuori ambito**

Attualmente, le seguenti funzonalità non sono supportate:

- **Analisi avanzata percorso**
- **Modifiche al percorso in tempo reale**
- **Orchestrazione tra percorsi**
- **Configurazione test A/B**
- **Trasformazioni dati complesse**
- **Creazione del contenuto del messaggio**

## Prompt di esempio

### Richieste comuni per la creazione di un percorso

Di seguito sono riportati alcuni esempi di prompt utili che gli utenti possono sfruttare per creare percorsi.

### Richieste di percorso attivate da eventi

**percorso di visite allo store:**

&quot;Crea un percorso che inizia quando un utente accede alla posizione del mio negozio. Invia una notifica push per accogliere gli utenti nello store. Attendi 2 giorni e controlla se l’utente ha un indirizzo e-mail valido. Se l’utente dispone di un indirizzo e-mail valido, invia un sondaggio e-mail per chiedere informazioni sulla sua esperienza di negozio. Se l’utente non dispone di un indirizzo e-mail valido, invia una notifica push per richiedere la registrazione.&quot;

**percorso post-acquisto:**

&quot;Crea un percorso che inizia quando un cliente effettua un acquisto online. Invia una notifica push per ringraziarli dell’acquisto. Quindi, verifica se sono membri fedeltà. Se l’utente è un membro dei premi fedeltà, invia una seconda notifica push con un codice di sconto del 10%. Se l’utente non è un membro dei premi fedeltà, invia un messaggio push per invitarlo a iscriversi al programma fedeltà. Attendi 2 giorni e invia un messaggio push di follow-up con un sondaggio sulla loro esperienza di acquisto.&quot;

**Promozione basata su eventi:**

&quot;Crea un percorso attivato quando il punteggio di gioco raggiunge 50. Invia un messaggio SMS ai membri del premio fedeltà che dichiarano di poter usufruire di una fetta gratuita di pizza dallo sponsor partner.&quot;

### Richieste di percorso mirate al pubblico

**Campagna stagionale:**

&quot;Voglio creare un percorso che si rivolga ad un pubblico di escursionisti. Voglio inviare un messaggio e-mail per avvisare il pubblico della mia prossima vendita di vacanze che include una varietà di elementi essenziali per le escursioni. Attendi 3 giorni dopo l’invio della prima e-mail e invia una seconda e-mail con un coupon del 15% con spedizione gratuita. Attendi 1 settimana e poi invia un terzo messaggio e-mail per mostrare il nostro nuovo sacco a pelo e la collezione di tende. Pianifica il percorso per iniziare il 20/12.&quot;

**Riconoscimento fedeltà:**

&quot;Crea un percorso di apprezzamento della fedeltà per i proprietari di SUV, tra cui una notifica push di ringraziamento con un’offerta di carwash gratuita e un promemoria di notifica push di follow-up se la prima notifica non viene interagita entro 1 giorno.&quot;

### Richieste aperte

Per gli utenti che iniziano senza considerare un percorso specifico:

- &quot;Vorrei creare un percorso&quot;
- &quot;Aiutami a creare un percorso&quot;
- &quot;Crea un percorso&quot;

L&#39;agente fornirà indicazioni ed esempi per aiutarti a definire i tuoi requisiti percorsi.

## Best practice

### Best practice per la richiesta di informazioni

Per massimizzare l’efficacia di Percorsi Create Agent, segui queste best practice:

1. **Specifica**: fornisci dettagli chiari sugli obiettivi del percorso, sul pubblico di destinazione e sulle azioni desiderate. Includi informazioni su canali, tempi e condizioni.
1. **Specificare l&#39;intervallo**: indicare chiaramente i periodi di attesa tra le azioni e l&#39;inizio del percorso.
1. **Definisci condizioni**: quando utilizzi la logica condizionale, spiega i criteri per ciascun percorso di diramazione.
1. **Includi canali**: specifica i canali di comunicazione da utilizzare (push, e-mail, SMS).
1. **Pianificazione menzione**: per i percorsi pianificati, fornisci la data e l&#39;ora di inizio desiderate.
1. **Azioni personalizzate**: se utilizzi azioni personalizzate nel flusso di lavoro, devi specificare che utilizzi un&#39;azione personalizzata insieme al nome esatto dell&#39;azione personalizzata. Esempio:
Quando un utente accede alla posizione del mio archivio, invia un messaggio di benvenuto utilizzando l’azione personalizzata ExternalPush. Attendi 2 giorni e invia un messaggio di follow-up utilizzando l’azione personalizzata ExternalEmail con un sondaggio sulla loro visita.
1. **Convalida espressioni**: verificare e convalidare tutte le espressioni create da Journey Agent per assicurarsi che vengano utilizzati i campi e i valori corretti.

### Best practice per l’impostazione

- **Definisci obiettivi chiari**: prima di creare percorsi, stabilisci obiettivi chiari (miglioramento della fidelizzazione, conversioni e coinvolgimento).
- **Prepara tipi di pubblico**: assicurati che i tipi di pubblico di destinazione siano già stati creati e correttamente segmentati.
- **Pianifica contenuto messaggio**: definire la strategia di messaggistica prima di creare il percorso.
- **Esperienza cliente**: progettare flussi di percorso che rispettino le preferenze del cliente ed evitino comunicazioni eccessive.

