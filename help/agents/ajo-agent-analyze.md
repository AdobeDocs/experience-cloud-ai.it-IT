---
title: Panoramica e guida utente di Percorsi Analyze Agent Skill
description: Guida completa alle competenze di Journey Agent Analyze, che consente agli utenti di analizzare i percorsi di marketing, rilevare i problemi, scoprire informazioni approfondite e ottimizzare il coinvolgimento dei clienti.
solution: Journey Optimizer
product: journey optimizer
role: Admin,User,Developer,Leader
source-git-commit: c9909616697ef319a307b5c8a1ee135204347844
workflow-type: tm+mt
source-wordcount: '986'
ht-degree: 0%

---


# Agente analisi percorso: panoramica abilità e guida utente

## Panoramica

Journey Agent consentirà agli utenti di Journey Optimizer di analizzare e ottimizzare i percorsi utilizzando un&#39;interfaccia in linguaggio naturale. Con Journey Agent, i professionisti possono identificare e risolvere rapidamente i conflitti di pianificazione e/o di pubblico, rilevare punti di abbandono degli utenti in un percorso e fornire informazioni o consigli. Consente ai professionisti di prendere decisioni basate sui dati, migliorare il coinvolgimento dei clienti e semplificare l’orchestrazione del percorso.

>[!AVAILABILITY]
>
>Il Journey Agent è disponibile per tutti i clienti che hanno accesso all’Assistente per l’intelligenza artificiale. Tuttavia, per utilizzare completamente le funzioni di Journey Agent, sono necessarie le seguenti autorizzazioni.
>
>**Visualizza Percorsi**: questa autorizzazione consente di utilizzare Journey Agent per visualizzare informazioni sul percorso direttamente nell&#39;Assistente IA.
>
>**Gestisci Percorsi**: con autorizzazione consente di utilizzare Journey Agent per creare nuovi percorsi direttamente nell&#39;Assistente IA.
>
>**Visualizza segmenti**: questa autorizzazione ti consente di utilizzare Journey Agent per visualizzare approfondimenti sui tipi di pubblico direttamente nell&#39;Assistente AI.
>
>**Gestisci segmenti**: con autorizzazione consente di utilizzare Journey Agent per creare nuovi tipi di pubblico direttamente nell&#39;Assistente IA.

![Esempio per AJO Agent](./images/ajo-agent/ajo-agent-sample.png)

## Casi d’uso

### Casi d’uso principali per Journey Agent Analyze

L’abilità Journey Agent Analyze offre una serie di funzionalità che possono essere utilizzate per ottimizzare le attività di marketing:

1. **Analisi Abbandono Percorso**

   - Identifica dove e perché i clienti abbandonano durante un percorso.
   - Rileva i pattern di comportamento del cliente che portano al disimpegno.
   - Utilizza le informazioni per perfezionare la progettazione del percorso e migliorare la conservazione.

1. **Analisi sovrapposizione pubblico Percorso**

   - Analizzare la sovrapposizione del pubblico in più percorsi.
   - Impedisci al pubblico di essere affaticato da un targeting eccessivo.
   - Ottimizza la segmentazione per garantire un coinvolgimento equilibrato.

1. **Analisi sovrapposizione pianificazione Percorsi**

   - Rileva i conflitti di tempistica tra percorsi pianificati che si rivolgono allo stesso pubblico.
   - Evita comunicazioni eccessive e migliora l&#39;efficienza della pianificazione.
   - Massimizza l’impatto sul pubblico garantendo che i percorsi vengano eseguiti in tempi ottimali.

1. **Informazioni operative**

   - Approfondimenti sul Percorso basati su prompt: visualizza informazioni operative sui percorsi, ad esempio &quot;mostrami tutti i percorsi live&quot;.

Per ciascuna di queste analisi, l&#39;agente non solo rileva i problemi, ma fornisce anche **consigli utili per risolverli**.


## Abilità nell’ambito e al di fuori dell’ambito

### **Nell&#39;Ambito**

Journey Agent Analyze supporta le seguenti funzionalità:

- **Query reattive**: consente agli utenti di porre domande specifiche sulle prestazioni del percorso, sull&#39;utilizzo del pubblico e sui conflitti di pianificazione.
- **Integrazione con altri agenti**: collabora con Audience Agent e Data Insights Agent per analisi più approfondite.
- **Struttura della risposta dell&#39;agente**: ragionamento (spiegazione della logica), riepilogo dell&#39;analisi (evidenziazione dei punti chiave), dettagli del problema (descrizione del problema) e consiglio (proposta dei passaggi successivi).

### **Fuori ambito**

Le seguenti funzionalità non sono attualmente supportate:

- **Creazione automatica Percorso**
- **Rilevamento delle anomalie in tempo reale**
- **Sovrapposizione canali**
- **Analisi delle voci di Percorso**
- **Analisi dei problemi tecnici**
- **Analisi affaticamento**

## Prompt di esempio / Prompt di esempio

### Richieste comuni per l&#39;analisi del Percorso

Di seguito sono riportati alcuni esempi di prompt utili che gli utenti possono utilizzare per esplorare, monitorare e risolvere problemi dei propri percorsi.

### Domande sul ciclo di vita del percorso

- &quot;Quando è stato pubblicato [Nome Percorso]?&quot;
- &quot;Quando è stato interrotto [Nome Percorso]?&quot;
- &quot;Elenca tutti i percorsi attualmente in modalità di test&quot;

### Domande risorsa percorso

- &quot;Quanti percorsi di vita ho?&quot;
- &quot;Dammi un elenco di tutti i percorsi ricorrenti pianificati e dei loro orari di esecuzione previsti.&quot;

### Informazioni su pubblico e Percorso

- &quot;Quali tipi di pubblico vengono utilizzati in più di X percorsi?&quot;
- &quot;Elenca tutti i percorsi che utilizzano il pubblico [nome pubblico].&quot;

### Analisi dell’abbandono

- &quot;Voglio analizzare l’abbandono per nodo per la campagna del 4 luglio percorso.&quot;
- &quot;Esegui un’analisi dell’abbandono per la campagna del 4 luglio percorso.&quot;
- &quot;Cos’è la perdita di profilo nel corso della campagna del 4° percorso di luglio?&quot;
- &quot;Mostra dove gli utenti abbandonano la campagna del 4 luglio percorso.&quot;

### Prompt analisi conflitti

Utilizza questi prompt per analizzare i potenziali conflitti tra percorsi, incluse le sovrapposizioni di pianificazione e pubblico:

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

### Best practice per la richiesta di assistenza

Per ottimizzare l’efficacia di Journey Agent Analyze, segui queste best practice:

1. **Essere specifici**: usa prompt chiari e concisi per ottenere informazioni mirate. Ad esempio, invece di chiedere &quot;Quali sono i miei percorsi?&quot;, specificare &quot;Elenca tutti i percorsi creati nell&#39;ultimo mese&quot;.
1. **Combina approfondimenti**: integra gli approfondimenti da Audience Agent e Data Insights Agent per una visualizzazione olistica delle prestazioni del percorso.
1. **Ottimizzazione iterativa**: utilizza l&#39;analisi di abbandono e sovrapposizione per perfezionare iterativamente la progettazione e la pianificazione del percorso.

### Best practice per l’installazione

- **Definisci obiettivi chiari**: prima di analizzare i percorsi, stabilisci obiettivi chiari (ad esempio, miglioramento della conservazione, aumento delle conversioni).
- **Monitora regolarmente**: pianifica revisioni regolari delle prestazioni del percorso per identificare tendenze e anomalie.
- **Ottimizza segmentazione**: assicurati che la segmentazione del pubblico sia bilanciata per evitare affaticamento e massimizzare il coinvolgimento.
