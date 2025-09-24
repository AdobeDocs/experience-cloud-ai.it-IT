---
title: IA nelle applicazioni Experience Cloud
description: Scopri in che modo le applicazioni Experience Cloud utilizzano l’intelligenza artificiale generativa (GenAI), l’Assistente all’intelligenza artificiale e l’intelligenza artificiale agentica.
source-git-commit: 58cce845f525e7762f32379a8db5791b677ae54f
workflow-type: tm+mt
source-wordcount: '645'
ht-degree: 0%

---

# IA in Experience Cloud

Ti diamo il benvenuto nella guida completa per le funzionalità di intelligenza artificiale nelle applicazioni Adobe Experience Cloud. Questa documentazione illustra come gli agenti AI, AI Assistant e Adobe generativi vengono integrati nei flussi di lavoro di Experience Cloud per accelerare la produttività e migliorare il processo decisionale.

## Elementi inclusi in questa guida

### Assistente AI

[L&#39;Assistente AI](./ai-assistant/ai-assistant-ui.md) è uno strumento intelligente di IA conversazionale e generativo che aumenterà la produttività e ridefinirà il lavoro nelle applicazioni basate su Adobe Experience Platform. Gli utenti possono acquisire conoscenze sui prodotti, risolvere i problemi e ottenere informazioni operative attraverso messaggi in linguaggio naturale. È inoltre possibile utilizzare l’Assistente IA per accedere agli agenti Adobe Experience Platform e ad altre funzionalità di intelligenza artificiale.

**Funzioni chiave:**

- **Interfaccia conversazionale**: opzioni di visualizzazione a schermo intero e barra per diverse preferenze del flusso di lavoro
- **Prompt di individuazione**: prompt preconfigurati organizzati per categoria (apprendimento, analisi, ottimizzazione)
- **Impostazione contesto**: configura le impostazioni di applicazione, sandbox e visualizzazione dati per le risposte mirate
- **Visualizzazione dati**: grafici interattivi per approfondimenti dati
- **Verifica risposta**: citazioni di Source, spiegazioni di ragionamento e meccanismi di feedback

### Agent Orchestrator

[Adobe Experience Platform Agent Orchestrator](./agents/agent-orchestrator.md) è il nuovo livello agente in Adobe Experience Platform. Progettata per sfruttare la ricca disponibilità di dati e le conoscenze dei clienti della piattaforma, Experience Platform Agent Orchestrator potenzia l&#39;intelligenza e il ragionamento alla base di esperti Adobe Experience Platform Agent appositamente creati, consentendo loro di eseguire attività complesse di processo decisionale e risoluzione dei problemi in modo rapido e su larga scala, il tutto con la supervisione umana. Quando fai domande o richiedi assistenza tramite il linguaggio naturale in un’interfaccia di conversazione come l’Assistente AI, Agent Orchestrator chiama automaticamente agenti specializzati per ottenere le risposte giuste. Agent Orchestrator ricorda la cronologia delle conversazioni e consente di basarsi sulle domande precedenti in modo naturale, senza dover ripetere il contesto, e combina le informazioni provenienti da più agenti per fornire risposte chiare e unificate.

**Componenti core:**

- **Motore di ragionamento**: crea piani dettagliati e regola gli approcci in base alle esigenze
- **Agenti specializzati**: agenti appositamente creati per attività e domini specifici
- **Knowledge Base**: accesso sicuro alle informazioni e alla documentazione di business intelligence

### Agenti specializzati

#### Audience Agent

Fornisce informazioni approfondite sui tipi di pubblico, tra cui:

- Rilevamento di cambiamenti significativi nelle dimensioni del pubblico
- Identificazione di tipi di pubblico duplicati
- Esplorazione dell’inventario del pubblico
- Recupero dimensioni pubblico

#### Data Insights Agent

Disponibile in Customer Journey Analytics, questo agente:

- Risponde alle domande sui dati utilizzando il linguaggio naturale
- Genera visualizzazioni rilevanti in Analysis Workspace
- Utilizza componenti dalla visualizzazione dati e dati effettivi

#### Journey Agent

Consente agli utenti di Journey Optimizer di:

- Analisi e ottimizzazione dei percorsi in linguaggio naturale
- Rilevare e risolvere i conflitti di pianificazione o pubblico
- Analisi delle prestazioni e dei punti di rilascio

#### Agente di supporto prodotto

Offre funzionalità self-service di debug e risoluzione dei problemi:

- Risolvere i problemi relativi alle funzioni di Adobe Experience Platform senza uscire dai flussi di lavoro
- Creare ticket di supporto con il contesto dalle interazioni dell’Assistente IA
- Controllare gli aggiornamenti dei ticket tramite l’Assistente AI

## Introduzione

### Requisiti di accesso

Per utilizzare l’Assistente AI e gli agenti Experience Platform, l’amministratore Adobe deve impostare le autorizzazioni appropriate:

- **Real-Time CDP e Adobe Journey Optimizer**: sono necessarie le autorizzazioni &quot;Abilita Assistente IA&quot; e &quot;Visualizza informazioni operative&quot; per le domande operative
- **Customer Journey Analytics**: accesso tramite il controllo di accesso di Customer Journey Analytics per domande relative a informazioni sul prodotto e sui dati
- **Adobe Experience Manager**: accesso tramite Adobe Admin Console

### Privacy e sicurezza

L’Assistente per l’intelligenza artificiale è stato creato con privacy, sicurezza e governance in prima linea:

- Nessun dato personale viene utilizzato per la formazione
- Tutti i criteri di controllo di accesso esistenti vengono rispettati
- Compatibilità HIPAA con Adobe Experience Platform Healthcare Shield
- Regole di conservazione di 30 giorni per i registri di interazione
- Isolamento dei dati specifici della sandbox

## Best practice

- **Specifica** nelle richieste per ottenere informazioni mirate
- **Verifica le risposte** utilizzando le citazioni di origine e le spiegazioni del ragionamento
- **Utilizza l&#39;impostazione del contesto** per garantire le origini dati rilevanti
- **Fornisci un feedback** per migliorare le prestazioni dell&#39;Assistente AI
- **Combina approfondimenti** da più agenti per un&#39;analisi completa

## Considerazioni giuridiche

- L’Assistente IA attualmente supporta solo la lingua inglese
- Verifica sempre le risposte in quanto i modelli di lingua possono commettere errori
- Rivedere le fasi di ragionamento e le spiegazioni fornite
- Invia feedback per qualsiasi problema o imprecisione

Questa guida fornisce tutto il necessario per utilizzare in modo efficace le funzionalità di intelligenza artificiale nelle applicazioni Experience Cloud, dalle interazioni di base all’orchestrazione avanzata degli agenti e ai flussi di lavoro specializzati.

