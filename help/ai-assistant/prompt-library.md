---
title: Libreria prompt dell'Assistente AI
description: Scopri i diversi tipi di prompt e pattern di prompt che è possibile utilizzare quando si esegue una query su Assistente IA.
source-git-commit: 4bb6da3fe1abee98446df62c94730274e0931493
workflow-type: tm+mt
source-wordcount: '811'
ht-degree: 3%

---

# Libreria prompt dell&#39;Assistente AI

Leggere questa guida per i diversi tipi di prompt che è possibile utilizzare nell&#39;Assistente IA.

## Agente Audience

Le sezioni seguenti forniscono esempi di prompt che puoi utilizzare con Audience Agent per esplorare e analizzare i tipi di pubblico. Questi includono modi per analizzare le caratteristiche del pubblico, rilevare tipi di pubblico duplicati, recuperare le dimensioni del pubblico e monitorare modifiche significative nelle dimensioni del pubblico nel tempo. Utilizza questi prompt per ottenere informazioni più approfondite e mantenere la qualità dei dati sul pubblico.

### Esplorazione del pubblico di conversazione

- &quot;Mostrami campi per acquirenti benestanti&quot;.
- &quot;Quali tipi di pubblico non sono stati attivati o utilizzati in alcuna campagna negli ultimi 30 giorni?&quot;
- &quot;Elenca tutti i tipi di pubblico che sono stati mappati sulle nuove destinazioni negli ultimi 3 mesi.&quot;

### Rilevare tipi di pubblico duplicati

- &quot;Ho tipi di pubblico con descrizioni identiche o simili?&quot;
- &quot;Identifica i tipi di pubblico che hanno le stesse regole ma nomi diversi.&quot;
- &quot;Mostra tutti i tipi di pubblico che hanno le stesse regole ma destinazioni di attivazione diverse.&quot;

### Recupera dimensione pubblico

- &quot;Qual è la dimensione attuale del mio pubblico &quot;Membri Gold-star in California_f153e1&quot;?&quot;
- &quot;Qual è il mio pubblico più grande?&quot;

### Rilevare cambiamenti significativi nelle dimensioni del pubblico

- &quot;Quale pubblico è aumentato di oltre il 20% nell’ultima settimana?&quot;
- &quot;Quali tipi di pubblico sono diminuiti di oltre il 15% nell’ultimo mese?&quot;
- &quot;Qual è il mio pubblico in più rapida crescita?&quot;

## Data Insights Agent

I seguenti prompt di esempio possono essere utilizzati con Data Insights Agent per analizzare i dati, identificare le tendenze e individuare informazioni fruibili.

### Visualizzazione dati

- &quot;Mostrami i profitti a settembre.&quot;
- &quot;Trend ordini a settembre.&quot;
- &quot;Mostra ricavi per area geografica in settembre&quot;.
- &quot;Quota di reddito per categoria di prodotto&quot;.
- &quot;Ordini per giorno della settimana, da gennaio a maggio.&quot;
- &quot;Mostra gli ordini per genere, da marzo a giugno.&quot;
- &quot;Qual è il profitto tra SKU da febbraio a maggio.&quot;
- &quot;Ricavi per nome del negozio in settembre.&quot;
- &quot;Quali sono stati i miei 10 SKU principali in base ai profitti a settembre?&quot;
- &quot;Percentuale di acquisti per mese dell&#39;anno.&quot;
- &quot;Profitto totale a settembre&quot;.

## Journey Agent

I prompt di esempio seguenti possono essere utilizzati con Journey Agent per analizzare i cicli di vita del percorso, gestire le risorse di percorso, acquisire informazioni approfondite sulle relazioni tra pubblico e percorso e rilevare i conflitti tra percorsi. Utilizza questi prompt per ottimizzare l’orchestrazione del percorso e risolvere i problemi in modo efficiente.

### Domande sul ciclo di vita del percorso

- &quot;Quando è stato pubblicato {JOURNEY_NAME}?&quot;
- &quot;Quando è stato interrotto {JOURNEY_NAME}?&quot;
- &quot;Elenca tutti i percorsi attualmente in modalità di test&quot;

### Domande sulle risorse del percorso

- &quot;Quanti percorsi di vita ho?&quot;
- &quot;Dammi un elenco di tutti i percorsi ricorrenti pianificati e dei loro orari di esecuzione previsti.&quot;

### Insight sul pubblico e sul percorso

- &quot;Quali tipi di pubblico vengono utilizzati in più di X percorsi?&quot;
- &quot;Elenca tutti i percorsi che utilizzano il pubblico {AUDIENCE_NAME}.&quot;

### Prompt di analisi del conflitto

Utilizza questi prompt per analizzare possibili conflitti tra percorsi, incluse le sovrapposizioni di pianificazione e pubblico:

+++Seleziona per visualizzare l’elenco

- &quot;È possibile eseguire un&#39;analisi completa dei conflitti per il percorso {JOURNEY_NAME} con informazioni sul tipo di conflitto (pianificazione/pubblico) con percorsi attivi/in esecuzione?&quot;
- &quot;Eseguire un&#39;analisi dei conflitti di pianificazione per il percorso {JOURNEY_NAME} con informazioni sul tipo di conflitto.&quot;
- &quot;Eseguire un&#39;analisi di sovrapposizione del pubblico per il percorso {JOURNEY_NAME} con informazioni sul tipo di conflitto.&quot;
- &quot;Esistono conflitti di pianificazione per il percorso {JOURNEY_NAME}?&quot;
- &quot;Mostra conflitti di sovrapposizione del pubblico per il percorso {JOURNEY_NAME}.&quot;
- &quot;Analizzare tutti i conflitti per il percorso {JOURNEY_NAME} con altri percorsi attivi.&quot;
- &quot;Quali sono i conflitti correnti per il percorso {JOURNEY_NAME}?&quot;
- &quot;Verificare se il percorso {JOURNEY_NAME} presenta conflitti di pubblico con altri percorsi.&quot;
- &quot;Verificare la presenza di conflitti di pianificazione che interessano il percorso {JOURNEY_NAME}.&quot;
- &quot;Desidero conoscere tutti i conflitti di percorso per {JOURNEY_NAME}.&quot;
- &quot;Esistono percorsi in conflitto con {JOURNEY_NAME} in base alla pianificazione o al pubblico?&quot;
- &quot;Identificare i tipi di conflitto per il percorso {JOURNEY_NAME} rispetto ai percorsi in esecuzione.&quot;
- &quot;Mostra tipi di pubblico sovrapposti per il percorso {JOURNEY_NAME} e altri percorsi.&quot;
- &quot;Evidenzia le sovrapposizioni di pianificazione tra il percorso {JOURNEY_NAME} e i percorsi live.&quot;
- &quot;Il percorso {JOURNEY_NAME} è in esecuzione in conflitto con altri percorsi?&quot;
- &quot;Rilevare ed elencare i conflitti per {JOURNEY_NAME}.&quot;
- &quot;Segnala tutti i tipi di conflitti per il percorso {JOURNEY_NAME}.&quot;
- &quot;Assegnami un raggruppamento dei conflitti (pianificazione e pubblico) per {JOURNEY_NAME}.&quot;
- &quot;{JOURNEY_NAME} ha conflitti che possono influire sulle prestazioni?&quot;
- &quot;Sono presenti conflitti attivi che interessano {JOURNEY_NAME}?&quot;
- &quot;Elenca i percorsi in conflitto con {JOURNEY_NAME} per pianificazione o pubblico.&quot;
- &quot;Il percorso {JOURNEY_NAME} ha attivato avvisi sui conflitti?&quot;
- &quot;Trovare potenziali conflitti di pubblico per il percorso {JOURNEY_NAME}.&quot;
- &quot;Analizzare il rischio di conflitto per il percorso {JOURNEY_NAME}.&quot;
- &quot;Specificare la diagnostica dei conflitti per {JOURNEY_NAME}.&quot;

+++

## Agente di supporto prodotto

L’agente di supporto del prodotto consente di risolvere i problemi, creare casi di supporto e tenere traccia dello stato dei ticket di supporto. Per ottenere assistenza, utilizza i prompt di esempio seguenti.

### Aiuto per la risoluzione dei problemi

- &quot;Perché il conteggio dei miei profili differisce in License Usage Dashboard (Dashboard di utilizzo della licenza) e nella home page di Experience Platform?&quot;
- &quot;Quali sono le ragioni per cui un percorso non si attiva?&quot;
- &quot;In che modo Adobe Experience Platform crea esperienze in tempo reale?&quot;
- &quot;Come si configurano e utilizzano gli avvisi in Adobe Experience Platform?&quot;
- &quot;Qual è il limite per i processi di segmentazione batch in Adobe Experience Platform Activation?&quot;
- &quot;Qual è il limite medio di ricchezza del profilo in Adobe Experience Platform Activation?&quot;

### Creazione di casi di supporto

- &quot;Crea un ticket di supporto.&quot;
- &quot;Puoi aiutarmi a creare un ticket di supporto?&quot;

### Tracciare l’avanzamento del caso

- &quot;Quali sono le ultime notizie sul mio caso E-12345?&quot;
- &quot;Qual è l&#39;aggiornamento del ticket E-67890?&quot;

