---
title: Panoramica e guida utente di Journey Agent
description: Guida completa a Journey Agent, che consente agli utenti di creare, analizzare e ottimizzare i percorsi di marketing utilizzando un’interfaccia in linguaggio naturale in Journey Optimizer.
solution: Journey Optimizer
product: journey optimizer
role: Admin,User,Developer,Leader
source-git-commit: 0e3839f829efc5670c235435d49ed5e49da2ed13
workflow-type: tm+mt
source-wordcount: '2147'
ht-degree: 18%

---


# Journey Agent: Panoramica e guida utente

## Introduzione a Journey Agent in Adobe Journey Optimizer

Journey Agent consente agli utenti di Journey Optimizer di creare, analizzare e ottimizzare percorsi di marketing utilizzando un’interfaccia in linguaggio naturale. Con l’agente Journey, i professionisti possono generare rapidamente percorsi, rilevare e risolvere conflitti di pianificazione o pubblico, analizzare le prestazioni e i tassi di abbandono e identificare i percorsi che funzionano meglio per replicarli in future campagne. Consente ai professionisti di prendere decisioni basate sui dati, migliorare il coinvolgimento dei clienti e semplificare l’orchestrazione del percorso.

Journey Agent si compone di due competenze principali:
- **Agente di creazione Percorso**: genera e configura percorsi di marketing tramite prompt in linguaggio naturale
- **Percorso Analizza agente**: analizza i percorsi, rileva i problemi, scopri informazioni e ottimizza il coinvolgimento dei clienti

&#x200B;---

&#x200B;# Percorsi Create Agent: panoramica delle abilità e guida utente

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

&#x200B;---

&#x200B;# Agente analisi percorso: panoramica abilità e guida utente

## Panoramica

Journey Agent consentirà agli utenti di Journey Optimizer di analizzare e ottimizzare i percorsi utilizzando un&#39;interfaccia in linguaggio naturale. Con Journey Agent, i professionisti possono identificare e risolvere rapidamente i conflitti di pianificazione e/o di pubblico, rilevare punti di abbandono degli utenti in un percorso e fornire informazioni o consigli. I professionisti saranno in grado di effettuare decisioni guidate dai dati, migliorare il coinvolgimento cliente e semplificare l’orchestrazione del percorso.

Per ulteriori informazioni e per scoprire subito l&#39;agente, consulta questa [panoramica](https://experienceleague.adobe.com/en/slides/journey-agent-overview).

>[!AVAILABILITY]
>
>Il Journey Agent è disponibile per tutti i clienti che hanno accesso all’Assistente per l’intelligenza artificiale. Tuttavia, per utilizzare completamente le funzioni di Journey Agent, sono necessarie le seguenti autorizzazioni:
>
>**Visualizza Percorsi**: questa autorizzazione ti consente di visualizzare approfondimenti sul percorso direttamente nell&#39;Assistente AI.
>
>**Gestisci Percorsi**: con autorizzazione consente di creare nuovi percorsi direttamente nell&#39;Assistente IA.
>
>**Visualizza segmenti**: questa autorizzazione ti consente di visualizzare approfondimenti sui tipi di pubblico direttamente nell&#39;Assistente AI.
>
>**Gestisci segmenti**: con autorizzazione consente di creare nuovi tipi di pubblico direttamente nell&#39;Assistente IA.

![Esempio per AJO Agent](./images/ajo-agent/ajo-agent-sample.png)

## Casi d’uso

### Principali casi d’uso dell’analisi dell’agente Journey

La capacità di analisi dell’agente Journey offre una gamma di funzionalità che possono essere sfruttate per ottimizzare le attività di marketing:

1. **Analisi fall-out del percorso**

   - Identifica il punto e il motivo per cui un percoso viene abbandonato dalla clientela.
   - Identifica schemi nel comportamento della clientela che portano a interrompere il coinvolgimento.
   - Utilizza gli insight per perfezionare i progetti di percorso e migliorare la conservazione.

1. **Analisi della sovrapposizione del pubblico del percorso**

   - Analizza la sovrapposizione del pubblico in diversi percorsi.
   - Evita la stanchezza del pubblico causata da targeting eccessivo.
   - Ottimizza la segmentazione per garantire un coinvolgimento equilibrato.

1. **Analisi della sovrapposizione della pianificazione del percorso**

   - Rileva conflitti temporali tra percorsi pianificati destinati allo stesso pubblico.
   - Evita l’eccessiva comunicazione e migliora l’efficienza della pianificazione.
   - Ottimizza l’impatto sul pubblico, garantendo che i percorsi vengano eseguiti nel momento migliore.

1. **Insight operativi**

   - Approfondimenti sul Percorso basati su prompt: visualizza informazioni operative sui percorsi, ad esempio &quot;mostrami tutti i percorsi live&quot;.

Per ciascuna di queste analisi, l&#39;agente non solo rileva i problemi, ma fornisce anche **consigli utili per risolverli**.

## Competenze rilevanti e non rilevanti per l’ambito

### **Rilevanti per l’ambito**

L’analisi dell’agente Journey supporta le seguenti funzionalità:

- **Query reattive**: consentono agli utenti di porre domande specifiche riguardanti le prestazioni del percorso, l’utilizzo del pubblico e i conflitti di pianificazione.
- **Integrazione con altri agenti**: collabora con Agente Audience e Agente Data Insights per analisi più approfondite.
- **Struttura della risposta dell&#39;agente**: ragionamento (spiegazione della logica), riepilogo dell&#39;analisi (evidenziazione dei punti chiave), dettagli del problema (descrizione del problema) e consiglio (proposta dei passaggi successivi).

### **Non rilevanti per l’ambito**

Attualmente, le seguenti funzonalità non sono supportate:

- **Creazione automatizzata del percorso**
- **Rilevamento di anomalie in tempo reale**
- **Sovrapposizione di canali**
- **Analisi dell’ingresso nel percorso**
- **Analisi di un problema tecnico**
- **Analisi della stanchezza**

## Campioni/esempi di prompt

### Prompt comuni per l’analisi del percorso

Di seguito sono disponibili alcuni esempi di prompt efficaci che gli utenti possono sfruttare per esplorare, monitorare e risolvere i problemi dei propri percorsi.

### Domande sul ciclo di vita del percorso

- &quot;Quando è stato pubblicato [Nome Percorso]?&quot;
- &quot;Quando è stato interrotto [Nome Percorso]?&quot;
- &quot;Elenca tutti i percorsi attualmente in modalità di test&quot;

### Domande sulle risorse del percorso

- &quot;Quanti percorsi di vita ho?&quot;
- &quot;Dammi un elenco di tutti i percorsi ricorrenti pianificati e dei loro orari di esecuzione previsti.&quot;

### Insight sul pubblico e sul percorso

- &quot;Quali tipi di pubblico vengono utilizzati in più di X percorsi?&quot;
- &quot;Elenca tutti i percorsi che utilizzano il pubblico [nome pubblico].&quot;

### Analisi dell’abbandono

- &quot;Voglio analizzare l’abbandono per nodo per la campagna del 4 luglio percorso.&quot;
- &quot;Esegui un’analisi dell’abbandono per la campagna del 4 luglio percorso.&quot;
- &quot;Cos’è la perdita di profilo nel corso della campagna del 4° percorso di luglio?&quot;
- &quot;Mostra dove gli utenti abbandonano la campagna del 4 luglio percorso.&quot;

### Prompt di analisi del conflitto

Utilizza questi prompt per analizzare possibili conflitti tra percorsi, incluse le sovrapposizioni di pianificazione e pubblico:

- &quot;È possibile eseguire un&#39;analisi completa dei conflitti per il nome del percorso [Percorso] con informazioni sul tipo di conflitto (pianificazione/pubblico) con percorsi attivi/in esecuzione?&quot;
- &quot;Eseguire un&#39;analisi dei conflitti di pianificazione per il percorso [Nome Percorso] con informazioni sul tipo di conflitto.&quot;
- &quot;Eseguire un&#39;analisi di sovrapposizione del pubblico per il percorso [Nome Percorso] con informazioni sul tipo di conflitto.&quot;
- &quot;Sono presenti conflitti di pianificazione per il percorso [Nome Percorso]?&quot;
- &quot;Mostra conflitti di sovrapposizione del pubblico per il percorso [Nome Percorso].&quot;
- &quot;Analizzare tutti i conflitti per il percorso [Nome Percorso] con altri percorsi attivi.&quot;
- &quot;Quali sono i conflitti correnti per il percorso [Nome Percorso]?&quot;
- &quot;Verificare se il nome del percorso [Percorso] contiene conflitti di pubblico con altri percorsi.&quot;
- &quot;Verificare la presenza di conflitti di pianificazione che interessano il percorso [Nome Percorso].&quot;
- &quot;Desidero conoscere tutti i conflitti di percorso per [Nome Percorso].&quot;
- &quot;I percorsi attivi sono in conflitto con [Nome Percorso] in base alla pianificazione o al pubblico?&quot;
- &quot;Identificare i tipi di conflitto per il percorso [Nome Percorso] rispetto ai percorsi in esecuzione.&quot;
- &quot;Mostra tipi di pubblico sovrapposti per il percorso [Nome Percorso] e altri percorsi.&quot;
- &quot;Evidenzia sovrapposizioni di pianificazione tra il percorso [Nome Percorso] e percorsi live.&quot;
- &quot;Il percorso [Nome Percorso] è in esecuzione in conflitto con altri percorsi?&quot;
- &quot;Rileva ed elenca i conflitti per [Nome Percorso].&quot;
- &quot;Segnala tutti i tipi di conflitti per il percorso [Nome Percorso].&quot;
- &quot;Assegnami un raggruppamento in conflitto (pianificazione e pubblico) per [Nome Percorso].&quot;
- &quot;Il nome del Percorso [] presenta conflitti che possono influire sulle prestazioni?&quot;
- &quot;Sono presenti conflitti attivi che interessano [Nome Percorso]?&quot;
- &quot;Elenca i percorsi in conflitto con [Nome Percorso] in base alla pianificazione o al pubblico.&quot;
- &quot;Il percorso [Nome Percorso] ha attivato avvisi sui conflitti?&quot;
- &quot;Trovare potenziali conflitti di pubblico per il nome del percorso [Percorso].&quot;
- &quot;Analizzare i rischi di conflitto per il nome del percorso [Percorso].&quot;
- &quot;Specificare la diagnostica dei conflitti per [Nome Percorso].&quot;

## Best practice

### Prompt per le best practice

Per ottimizzare l’efficacia dell’analisi dell’agente Journey, segui queste best practice:

1. **Richieste specifiche**: utilizza prompt chiari e concisi per ottenere insight mirati. Ad esempio, invece di chiedere &quot;Quali sono i miei percorsi?&quot;, specificare &quot;Elenca tutti i percorsi creati nell&#39;ultimo mese&quot;.
1. **Combina gli insights**: integra gli insight di Agente Audience e Agente Data Insights per una vista olistica delle prestazioni del percorso.
1. **Miglioramento progressivo**: utilizza le analisi di fall-out e sovrapposizione per perfezionare in modo progressivo il progetto e la pianificazione del percorso.

### Impostare le best practice

- **Definisci obiettivi chiari**: prima di analizzare i percorsi, stabilisci obiettivi precisi (per esempio migliorare la conservazione, aumentare le conversioni).
- **Monitora regolarmente**: pianifica revisioni regolari delle prestazioni del percorso per identificare tendenze e anomalie.
- **Ottimizza la segmentazione**: assicurati che la segmentazione del pubblico sia equilibrata, per evitare stanchezza e ottimizzare il coinvolgimento.

&#x200B;---

## Diapositive e presentazioni

>[!NOTE]
>
>Le diapositive e il materiale per le presentazioni di Journey Agent saranno disponibili qui. Controlla di nuovo a breve se ci sono aggiornamenti.
