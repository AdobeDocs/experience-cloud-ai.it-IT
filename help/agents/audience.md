---
title: Agente Audience
description: Scopri come utilizzare Audience Agent per creare tipi di pubblico, visualizzarne le modifiche, rilevare tipi di pubblico duplicati e visualizzarne le informazioni.
source-git-commit: 4bb6da3fe1abee98446df62c94730274e0931493
workflow-type: tm+mt
source-wordcount: '816'
ht-degree: 2%

---


# Agente Audience

>[!AVAILABILITY]
>
>Audience Agent è disponibile per tutti i clienti che hanno accesso all’Assistente per l’intelligenza artificiale. Tuttavia, per utilizzare completamente le funzioni di Audience Agent, sono necessarie le seguenti autorizzazioni.
>
>**Visualizza segmenti**: questa autorizzazione ti consente di utilizzare Audience Agent per visualizzare approfondimenti sui tipi di pubblico direttamente nell&#39;Assistente AI.
>
>**Gestisci segmenti**: con autorizzazione consente di utilizzare Audience Agent per creare nuovi tipi di pubblico direttamente nell&#39;Assistente IA.

Audience Agent consente di visualizzare informazioni sui tipi di pubblico, tra cui il rilevamento di modifiche significative nelle dimensioni del pubblico, il rilevamento di tipi di pubblico duplicati, l’esplorazione dell’inventario dei tipi di pubblico e il recupero delle dimensioni dei tipi di pubblico.

## Casi d’uso supportati

Audience Agent nell’Assistente IA supporta i seguenti casi d’uso:

- Trova la dimensione del pubblico e rileva cambiamenti significativi nella dimensione del pubblico

   - Questo consente di trovare tipi di pubblico che sono improvvisamente cresciuti o si sono ridotti, per analizzare meglio i potenziali cambiamenti di mercato

- Rilevare tipi di pubblico duplicati

   - Questo consente di ridurre le ridondanze con il pubblico creato

- Trova i tipi di pubblico in base agli attributi completi o parziali denominati

   - Questo consente di navigare più facilmente nel tuo inventario del pubblico

- Scopri i campi XDM da utilizzare per definire un pubblico

   - Questa abilità ti consente di identificare più facilmente i campi giusti da utilizzare nel pubblico in base al contesto e alla rilevanza

Audience Agent non supporta **attualmente** le seguenti funzionalità:

- Creazione di un pubblico basato sulla conoscenza

   - La creazione di un pubblico basato sulla conoscenza sta creando un pubblico in base agli attributi e agli eventi forniti
   - Inoltre, puoi stimare la dimensione potenziale del pubblico prima di crearlo. Questo consente di eseguire rapidamente l’iterazione sul pubblico più efficace prima che sia pronto per l’attivazione
   - Il supporto per questa funzione sarà presto disponibile

- Esplorazione del pubblico basata sugli obiettivi

   - L’esplorazione del pubblico basata sugli obiettivi consente di scoprire set di dati e profili rilevanti allineati a un obiettivo di business applicando modelli di apprendimento automatico come la propensione all’acquisto o alla conversione.

Inoltre, quando utilizzi Audience Agent, tieni presente i seguenti vincoli:

- Audience Agent richiede almeno 24 ore per elaborare i tuoi dati

   - **impossibile** ad esempio disporre di una query per la ricerca di dati nelle ultime 24 ore. Dovrai controllare almeno nelle ultime 48 ore.

- Audience Agent supporta solo tipi di pubblico basati su **persone** che vengono valutati utilizzando la segmentazione batch

## Prompt di esempio

Negli esempi seguenti vengono illustrati i prompt di esempio e le risposte per Audience Agent.

### Esplorazione del pubblico di conversazione

Mostrami i campi per gli acquirenti benestanti.

+++ Risposta

![L&#39;Assistente AI mostra una tabella che mostra i campi rilevanti per gli acquirenti benestanti.](./images/audience/affluent-buyers.png)

+++

Quali tipi di pubblico non sono stati attivati o utilizzati in alcuna campagna negli ultimi 30 giorni?

+++ Risposta

![L&#39;Assistente AI mostra una tabella che mostra i tipi di pubblico che non sono stati attivati o utilizzati nelle campagne negli ultimi 30 giorni.](./images/audience/not-activated.png)

+++

Elenca tutti i tipi di pubblico che sono stati mappati sulle nuove destinazioni negli ultimi 3 mesi.

+++ Risposta

![L&#39;Assistente AI elenca il pubblico mappato a una nuova destinazione negli ultimi 3 mesi.](./images/audience/new-destination.png)

+++

### Rilevare tipi di pubblico duplicati

Ho tipi di pubblico con descrizioni identiche o simili?

+++ Risposta

![L&#39;Assistente AI visualizza una tabella contenente la definizione del segmento e i nomi dei tipi di pubblico con le stesse definizioni del segmento.](./images/audience/similar-descriptions.png)

+++

Identifica i tipi di pubblico che hanno le stesse regole ma nomi diversi.

+++ Risposta

![L&#39;Assistente di IA visualizza una tabella contenente i nomi dei tipi di pubblico che condividono le stesse regole di pubblico.](./images/audience/same-rules-different-names.png)

+++

Mostra tutti i tipi di pubblico che hanno le stesse regole ma destinazioni di attivazione diverse.

+++ Risposta

![L&#39;Assistente AI mostra che non sono presenti definizioni di segmenti duplicate in destinazioni diverse.](./images/audience/same-rules-different-destinations.png)

+++

### Recupera dimensione pubblico

Qual è la dimensione attuale del mio pubblico &quot;Membri Gold-star in California_f153e1&quot;?

+++ Risposta

![L&#39;Assistente di IA indica le dimensioni correnti del pubblico a cui è stato chiesto di fornire informazioni.](./images/audience/current-size.png)

+++

Qual è il mio pubblico più grande?

+++ Risposta

![L&#39;Assistente AI fornisce informazioni sul pubblico con il maggior numero di profili, inclusi nome e ID pubblico.](./images/audience/largest-audience.png)

+++

### Rilevare cambiamenti significativi nelle dimensioni del pubblico

Quali tipi di pubblico sono aumentati di oltre il 20% nell’ultima settimana?

+++ Risposta

![L&#39;Assistente IA visualizza una tabella che elenca i nomi di tutti i tipi di pubblico che corrispondono alla query. Mostra inoltre l&#39;aumento percentuale, la dimensione corrente del pubblico e la dimensione precedente del pubblico.](./images/audience/increase-past-week.png)

+++

Quali tipi di pubblico sono diminuiti di oltre il 10% nell’ultimo mese?

+++ Risposta

![L&#39;Assistente IA visualizza una tabella che elenca i nomi di tutti i tipi di pubblico che corrispondono alla query. Vengono inoltre visualizzate la dimensione del pubblico corrente, la dimensione del pubblico precedente e la data della dimensione del pubblico precedente.](./images/audience/decrease-month.png)

+++

Qual è il mio pubblico in più rapida crescita?

+++ Risposta

![L&#39;Assistente AI indica il nome del pubblico in più rapida crescita, nonché le dimensioni correnti e la percentuale di crescita.](./images/audience/fastest-growing.png)

+++

## Passaggi successivi

Dopo aver letto questa guida, avrai una migliore comprensione di Audience Agent e delle funzioni che supporta. Per ulteriori informazioni sugli agenti in Adobe Experience Platform, leggere la [panoramica di Agent Orchestrator](./agent-orchestrator.md).

