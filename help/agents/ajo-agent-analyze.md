---
title: Panoramica e guida utente di Percorsi Analyze Agent Skill
description: Guida completa alle abilità di analisi dell’agente Journey, che consente agli utenti di analizzare i percorsi di marketing, rilevare problemi, scoprire approfondimenti e ottimizzare il coinvolgimento cliente.
solution: Journey Optimizer
product: journey optimizer
role: Admin,User,Developer,Leader
source-git-commit: 26b579471b591d3c436f4275d07303d297e0fbf8
workflow-type: tm+mt
source-wordcount: '979'
ht-degree: 38%

---


# Agente analisi percorso: panoramica abilità e guida utente

## Panoramica

Journey Agent consentirà agli utenti di Journey Optimizer di analizzare e ottimizzare i percorsi utilizzando un&#39;interfaccia in linguaggio naturale. Con Journey Agent, i professionisti possono identificare e risolvere rapidamente i conflitti di pianificazione e/o di pubblico, rilevare punti di abbandono degli utenti in un percorso e fornire informazioni o consigli. I professionisti saranno in grado di effettuare decisioni guidate dai dati, migliorare il coinvolgimento cliente e semplificare l’orchestrazione del percorso.

Per ulteriori informazioni e per scoprire subito l&#39;agente, consulta questa [panoramica](https://experienceleague.adobe.com/it/slides/journey-agent-overview).

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

