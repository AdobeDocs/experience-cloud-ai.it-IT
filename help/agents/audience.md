---
title: Agente Audience
description: Scopri come utilizzare Audience Agent per creare tipi di pubblico, visualizzarne le modifiche, rilevare tipi di pubblico duplicati e visualizzarne le informazioni.
TQID: https://experienceleague.adobe.com/574QhqKI0YDoPHD9BFmB6jl-HET3zVom3eD4cJQABSE
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: f8a45b24-4be7-4f1b-909b-60d06b483a20
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
  - id: eb30f47f-d87a-400f-8f78-63ce7979ff56
source-git-commit: dd7883d8eccab3b0f006d55a850248e1c347d7e7
workflow-type: tm+mt
source-wordcount: 1242
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

>[!SLIDE](audience-agent-overview)

## Casi d’uso supportati

Audience Agent nell’Assistente IA supporta i seguenti casi d’uso:

- Esplorare il pubblico in modo conversazionale
   - Trovare le dimensioni dei tipi di pubblico esistenti
   - Cerca tipi di pubblico basati su attributi completi o parziali denominati
   - Rilevare tipi di pubblico duplicati
   - Scopri i campi XDM da utilizzare per definire un pubblico
- Rilevare cambiamenti significativi nelle dimensioni del pubblico
   - Questo consente di trovare tipi di pubblico che sono improvvisamente cresciuti o si sono ridotti, per analizzare meglio i potenziali cambiamenti di mercato
- Creazione di un pubblico
   - Questa abilità ti consente di creare un pubblico in base agli attributi e agli eventi forniti
   - Inoltre, questa abilità ti consente di stimare le dimensioni potenziali di un pubblico prima di crearlo, consentendoti di eseguire rapidamente l’iterazione del pubblico più efficace prima che sia pronto per essere attivato

<!--
  - Find your audience size and detect significant changes in audience size
  - This lets you find audiences that have suddenly grown or shrunk, letting you better analyze potential market changes
- Detect duplicate audiences
  - This lets you reduce redundancies with your created audiences
- Find audiences based on full or partial attributes named
  - This lets you more easily navigate through your audience inventory
- Discover XDM fields you can use to define an audience
  - This skill lets you more easily identify the right fields to use in your audience based on context and relevance 
-->

Audience Agent non supporta **attualmente** la seguente funzionalità:

- Esplorazione del pubblico basata sugli obiettivi
   - L’esplorazione del pubblico basata sugli obiettivi consente di scoprire set di dati e profili rilevanti allineati a un obiettivo di business applicando modelli di apprendimento automatico come la propensione all’acquisto o alla conversione.

Inoltre, quando utilizzi Audience Agent, tieni presente i seguenti vincoli:

- Audience Agent richiede almeno 24 ore per elaborare i tuoi dati
   - **impossibile** ad esempio disporre di una query per la ricerca di dati nelle ultime 24 ore. Dovrai controllare almeno nelle ultime 48 ore.
- Audience Agent supporta solo i seguenti tipi di pubblico:
   - **People-based** audiences that are evaluated using batch segmentation
   - **Account-based** audiences for the following use cases:
      - Conversational audience exploration
      - Duplicate audience detection

## Sample prompts

The following examples demonstrate sample prompts and responses for the Audience Agent.

### Conversational audience exploration

Show me fields for affluent buyers.

+++ Risposta

![The AI Assistant shows a table displaying fields that are relevant to affluent buyers.](./images/audience/affluent-buyers.png)

+++

Which audiences have not been activated or used in any campaign in the last 30 days?

+++ Risposta

![The AI Assistant shows a table that displays audiences that haven&#39;t been activated or used in campaigns in the last 30 days.](./images/audience/not-activated.png)

+++

List all the audiences that have been mapped to new destinations in the last 3 months.

+++ Risposta

![The AI Assistant lists the one audience that has been mapped to a new destination in the last 3 months.](./images/audience/new-destination.png)

+++

Which account audience has the largest audience size and what is that size?

+++ Risposta

![The AI Assistant shows a table that displays the largest account audiences.](./images/audience/largest-account-audience.png)

+++

### Rilevare tipi di pubblico duplicati

Do I have any audiences with identical or similar descriptions?

+++ Risposta

![The AI Assistant displays a table that contains the segment definition and the names of the audiences with the same segment definitions.](./images/audience/similar-descriptions.png)

+++

Identify audiences that have the same rules but have different names.

+++ Risposta

![The AI Assistant displays a table that contains the names of audiences that share the same audience rules.](./images/audience/same-rules-different-names.png)

+++

Show me all the audiences that have the same rules but different activation destinations.

+++ Risposta

![The AI Assistant shows that there are no duplicate segment definitions to different destinations.](./images/audience/same-rules-different-destinations.png)

+++

Identify account audiences that have the same rules but have different names.

+++ Risposta

![The AI Assistant displays a table that contains the names and IDs of account audiences that share the same audience rules.](./images/audience/duplicate-account-audience.png)

+++

### Recupera dimensione pubblico

What is the current size of my audience &quot;Gold-star Members in California_f153e1&quot;?

+++ Risposta

![The AI Assistant states the current size of the audience that was asked about.](./images/audience/current-size.png)

+++

What is my biggest audience?

+++ Risposta

![The AI Assistant gives information about the audience with the most profiles, including name and audience ID.](./images/audience/largest-audience.png)

+++

### Rilevare cambiamenti significativi nelle dimensioni del pubblico

Which audiences have increased in size by more than 20% in the last week?

+++ Risposta

![The AI Assistant displays a table that lists the names of all the audiences that match the query. It also shows the percentage increase, the current audience size, as well as the former audience size.](./images/audience/increase-past-week.png)

+++

Which audiences have decreased in size by more than 10% in the last month?

+++ Risposta

![The AI Assistant displays a table that lists the names of all the audiences that match the query. It also shows the current audience size, the former audience size, as well as the date of the old audience size.](./images/audience/decrease-month.png)

+++

What is my fastest growing audience?

+++ Risposta

![The AI Assistant states the name of the fastest growing audience, as well as the current size and the percentage of growth.](./images/audience/fastest-growing.png)

+++

### Creazione di un pubblico

>[!AVAILABILITY]
>
>You can only use the create audience skill if you are part of the Agent Orchestrator Explorer program. For more information, contact Adobe Customer Care.

When you create an audience with Audience Agent, AI Assistant will guide you through a plan. For example, you can ask to &quot;Create an audience made up of people who live in California&quot;. AI Assistant then lists the plan that it will undertake to create the audience.

+++ Risposta

![The AI Assistant shows the plan to create an audience.](./images/audience/audience-create-plan.png)

+++

This plan is made up of three steps:

1. [Identify audience characteristics](#identify)
2. [Estimate audience size](#estimate)
3. [Create and persist a new audience](#create)

#### Identify audience characteristics {#identify}

![Step 1 of the plan, which is to identify audience characteristics.](./images/audience/plan-step-1.png){align="center" width="80%"}

Dopo aver accettato il piano, l’Assistente AI acquisirà le caratteristiche del pubblico in base alla query iniziale.

+++ Risposta

![La definizione del pubblico basata sulla query utente.](./images/audience/audience-create-definition.png)

Per questa query, l’Assistente AI genera il Profile Query Language (PQL) rilevante che cercherà le persone che vivono in California. In questo caso d’uso, la query PQL sarà simile alla seguente:

```sql
homeAddress.state.equals("California", false)
```

Per ulteriori informazioni su PQL, leggere la [panoramica di PQL](https://experienceleague.adobe.com/it/docs/experience-platform/segmentation/pql/overview).

+++

Se la definizione del pubblico dell’Assistente AI è corretta, puoi approvare e passare al passaggio successivo.

#### Stimare la dimensione del pubblico {#estimate}

![Passaggio 2 del piano, che consiste nel stimare la dimensione del pubblico potenziale.](./images/audience/plan-step-2.png){align="center" width="80%"}

Dopo aver approvato le caratteristiche del pubblico identificato, AI Assistant stimerà le dimensioni del pubblico potenziale e i dettagli di definizione del pubblico.

+++ Risposta

![Viene visualizzata la stima di esempio per il pubblico potenziale. Vengono visualizzate la dimensione stimata e la definizione del segmento.](./images/audience/audience-create-estimate.png)

+++

Se la dimensione stimata è corretta, puoi approvare e passare al passaggio successivo.

#### Creare e mantenere un nuovo pubblico {#create}

![Passaggio 3 del piano, che consiste nel completare la creazione del pubblico.](./images/audience/plan-step-3.png){align="center" width="80%"}

Infine, se le caratteristiche e le dimensioni del pubblico sono corrette, puoi approvare o rifiutare la creazione del pubblico.

+++ Risposta

Innanzitutto, puoi esaminare il pubblico proposto tramite la griglia dati fornita.

![Viene visualizzata la schermata di revisione.](./images/audience/audience-create-review.png)

Se il pubblico è corretto, puoi accettare la proposta selezionando **[!UICONTROL Crea]** per completare la creazione del pubblico.

![Viene visualizzata la proposta completa per il pubblico.](./images/audience/audience-create-proposal.png)

+++

Il pubblico viene ora creato.

![La proposta di pubblico è stata accettata e il pubblico è stato creato.](./images/audience/audience-finish-create.png){align="center" width="80%"}

## Passaggi successivi

Dopo aver letto questa guida, avrai una migliore comprensione di Audience Agent e delle funzioni che supporta. Per ulteriori informazioni sugli agenti in Adobe Experience Platform, leggere la [panoramica di Agent Orchestrator](./agent-orchestrator.md).

