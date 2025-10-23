---
title: IA nelle applicazioni Experience Cloud
description: Scopri come le applicazioni Experience Cloud utilizzano l’IA generativa (GenAI), l’Assistente IA e l’IA agentica.
source-git-commit: a19c891d1a17c9112aff3d9a52daa94ad162a553
workflow-type: tm+mt
source-wordcount: '802'
ht-degree: 13%

---

# IA in Experience Cloud

Ti diamo il benvenuto nella guida completa per le funzionalità di intelligenza artificiale nelle applicazioni Adobe Experience Cloud. Questa documentazione illustra come gli agenti AI, AI Assistant e Adobe generativi vengono integrati nei flussi di lavoro di Experience Cloud per accelerare la produttività e migliorare il processo decisionale.

## Elementi inclusi in questa guida

### Assistente IA

[L&#39;Assistente AI](./ai-assistant/ai-assistant-ui.md) è uno strumento intelligente di IA conversazionale e generativo che aumenterà la produttività e ridefinirà il lavoro nelle applicazioni basate su Adobe Experience Platform. Gli utenti possono acquisire conoscenze sui prodotti, risolvere i problemi e ottenere informazioni operative attraverso messaggi in linguaggio naturale. È inoltre possibile utilizzare l’Assistente IA per accedere agli agenti Adobe Experience Platform e ad altre funzionalità di intelligenza artificiale.

**Funzioni chiave:**

- **Interfaccia conversazionale**: puoi scegliere tra un&#39;interfaccia a schermo intero e un&#39;interfaccia di visualizzazione della barra per adattarsi alle preferenze del flusso di lavoro.
- **Prompt di individuazione**: l&#39;Assistente IA fornisce prompt preconfigurati organizzati per categorie quali Apprendi, Analizza e Ottimizza.
- **Impostazione contesto**: è possibile configurare le impostazioni di applicazione, sandbox e visualizzazione dati per ricevere risposte personalizzate alle proprie esigenze.
- **Visualizzazione dati**: lo strumento fornisce grafici e grafici interattivi che consentono di ottenere informazioni dai dati.
- **Verifica risposta**: tutte le risposte includono citazioni di origine, spiegazioni del ragionamento dell&#39;intelligenza artificiale e meccanismi per fornire feedback.


### Agent Orchestrator

[Adobe Experience Platform Agent Orchestrator](./agents/agent-orchestrator.md) è il nuovo livello agente in Adobe Experience Platform. Progettato per sfruttare la ricca disponibilità di dati e le conoscenze della clientela della piattaforma, Agent Orchestrator di Experience Platform potenzia le informazioni e il ragionamento alla base degli Agenti esperti di Adobe Experience Platform appositamente creati, consentendo loro di eseguire complesse attività decisionali e di risoluzione dei problemi in modo rapido e su larga scala, sempre con intervento umano. Quando poni domande o richiedi assistenza tramite il linguaggio naturale in un’interfaccia conversazionale come l’Assistente IA, Agent Orchestrator richiama automaticamente ad agenti specializzati per ottenere le risposte giuste. Agent Orchestrator ricorda la cronologia delle conversazioni e consente di basarsi sulle domande precedenti in modo naturale, senza dover ripetere il contesto, e combina le informazioni provenienti da più agenti per fornire risposte chiare e unificate.

**Componenti core:**

- **Motore di ragionamento**: crea piani dettagliati e regola gli approcci in base alle esigenze
- **Agenti specializzati**: agenti appositamente creati per attività e domini specifici
- **Knowledge Base**: accesso sicuro alle informazioni e alla documentazione di business intelligence

### Agenti specializzati

#### Agente Audience

Audience Agent fornisce informazioni approfondite sui tipi di pubblico, tra cui:

- Rilevamento di cambiamenti significativi nelle dimensioni del pubblico.
- Identificazione di tipi di pubblico duplicati.
- Esplorazione dell’inventario del pubblico.
- Recupero dimensioni pubblico.

#### Data Insights Agent

Disponibile in Customer Journey Analytics, il Data Insights Agent:

- Risponde a domande sui dati utilizzando il linguaggio naturale.
- Genera visualizzazioni rilevanti in Analysis Workspace.
- Utilizza componenti dalla visualizzazione dati e dati effettivi.

#### Journey Agent

Journey Agent consente agli utenti di Adobe Journey Optimizer di:

- Analizzare e ottimizzare i percorsi utilizzando il linguaggio naturale.
- Rileva e risolvi i conflitti di pianificazione o pubblico.
- Analizzare le prestazioni e i punti di rilascio.

#### Agente di supporto prodotto

Utilizzare il Product Support Agent per il debug self-service e la risoluzione dei problemi:

- Risolvere i problemi relativi alle funzioni di Adobe Experience Platform senza uscire dai flussi di lavoro.
- Crea ticket di supporto con il contesto dalle interazioni dell’Assistente IA.
- Controlla gli aggiornamenti dei ticket tramite l’Assistente AI.

## Introduzione

### Requisiti di accesso

Per utilizzare l’Assistente AI e gli agenti Experience Platform, l’amministratore Adobe deve impostare le autorizzazioni appropriate:

- Per utilizzare l’Assistente AI in Real-Time CDP e Adobe Journey Optimizer, è necessario disporre dell’autorizzazione &quot;Abilita Assistente AI&quot; e dell’autorizzazione &quot;Visualizza informazioni operative&quot; per accedere alle domande operative.
- L’accesso a AI Assistant in Customer Journey Analytics viene gestito tramite Customer Journey Analytics Access Control, che consente di porre domande relative sia alla conoscenza del prodotto che all’approfondimento dei dati.
- Per Adobe Experience Manager, puoi accedere all’Assistente AI tramite le autorizzazioni impostate in Adobe Admin Console.

### Privacy e sicurezza

L’Assistente per l’intelligenza artificiale è stato creato con privacy, sicurezza e governance in prima linea:

- Nessun dato personale viene utilizzato per la formazione.
- Vengono rispettati tutti i criteri di controllo di accesso esistenti.
- Compatibile con HIPAA se utilizzato con Adobe Experience Platform Healthcare Shield.
- Regole di conservazione di 30 giorni per i registri di interazione.
- Isolamento dei dati specifico per la sandbox.

## Best practice

Per ottenere il massimo valore dall’esperienza di AI Assistant, segui queste best practice:

- **Specifica** nelle richieste per ottenere informazioni mirate e rilevanti dall&#39;Assistente AI.
- **Verifica le risposte** esaminando le citazioni di origine e le spiegazioni di ragionamento fornite dall&#39;Assistente di IA.
- **Utilizza l&#39;impostazione del contesto** per assicurarti che per le tue domande vengano utilizzate le origini dati più rilevanti.
- **Fornisci un feedback** per migliorare le prestazioni e la precisione dell&#39;Assistente AI nel tempo.
- **Combina le informazioni** provenienti da più agenti per ottenere un&#39;analisi più completa e accurata.

## Considerazioni giuridiche

Quando si utilizza AI Assistant, è importante essere a conoscenza delle principali considerazioni legali e pratiche. Attualmente, l’Assistente AI supporta solo le risposte in inglese. Presta sempre attenzione alla verifica delle informazioni fornite, in quanto i modelli linguistici possono occasionalmente commettere errori. Utilizza i passaggi di ragionamento e le spiegazioni incluse nelle risposte per comprendere meglio le risposte che ricevi. In caso di problemi o imprecisioni, invia un feedback per contribuire a migliorare l’Assistente AI nel tempo.
