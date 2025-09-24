---
title: Adobe Experience Platform Agent Orchestrator
description: Informazioni su Adobe Experience Platform Agent Orchestrator.
source-git-commit: 860b0f2414dc006c23fedcd7b0e29727fc0641d4
workflow-type: tm+mt
source-wordcount: '916'
ht-degree: 0%

---

# Adobe Experience Platform Agent Orchestrator

Adobe Experience Platform Agent Orchestrator è il nuovo livello di agente in Adobe Experience Platform. Progettata per sfruttare la ricca disponibilità di dati e le conoscenze dei clienti della piattaforma, Experience Platform Agent Orchestrator potenzia l&#39;intelligenza e il ragionamento alla base di esperti Adobe Experience Platform Agent appositamente creati, consentendo loro di eseguire attività complesse di processo decisionale e risoluzione dei problemi in modo rapido e su larga scala, il tutto con la supervisione umana. Quando fai domande o richiedi assistenza tramite il linguaggio naturale in un’interfaccia di conversazione come l’Assistente AI, Agent Orchestrator chiama automaticamente agenti specializzati per ottenere le risposte giuste. Agent Orchestrator ricorda la cronologia delle conversazioni e consente di basarsi sulle domande precedenti in modo naturale, senza dover ripetere il contesto, e combina le informazioni provenienti da più agenti per fornire risposte chiare e unificate.

Puoi completare flussi di lavoro end-to-end complessi tramite un’interfaccia di conversazione intuitiva senza dover sapere quali agenti lavorano dietro le quinte. Il sistema comprende i tuoi obiettivi, crea piani dettagliati e regola il suo approccio in base alle tue esigenze. Puoi esplorare il pannello di ragionamento per visualizzare il processo di pensiero passo per passo e capire meglio come vengono gestite le richieste. Con Agent Orchestrator, puoi gestire flussi di lavoro complessi e ottimizzare le strategie nelle applicazioni Adobe Experience Cloud.

Leggi questo documento per scoprire di più su Agent Orchestrator.

## Componenti di Agent Orchestrator {#components}

Agent Orchestrator è costituito da diverse parti chiave, tra cui l’interfaccia di conversazione dell’Assistente di intelligenza artificiale, un motore di ragionamento per il processo decisionale e la pianificazione, agenti Adobe Experience Platform specializzati e una knowledge base che fornisce l’accesso alle informazioni rilevanti.

![Architettura di marketing di Agent Orchestrator.](./images/agent-orchestrator/agentic-architecture.png)

### Interfaccia di conversazione dell&#39;Assistente AI {#ai-assistant}

L’Assistente AI è un’esperienza di conversazione che puoi utilizzare per accelerare i flussi di lavoro nelle applicazioni Adobe. È possibile utilizzare l’Assistente AI per comprendere meglio la conoscenza del prodotto, risolvere i problemi o eseguire ricerche attraverso le informazioni e trovare informazioni operative. L’Assistente AI supporta Experience Platform, Real-Time Customer Data Platform, Adobe Journey Optimizer e Customer Journey Analytics. È possibile utilizzare l’Assistente IA per accedere agli agenti di Experience Platform e ad altre funzionalità di intelligenza artificiale.

Per ulteriori informazioni, leggere la [Guida all&#39;interfaccia utente dell&#39;Assistente IA](../ai-assistant/ai-assistant-ui.md).

### Motore di ragionamento {#reasoning-engine}

Il motore di ragionamento interpreta i tuoi obiettivi in base alle richieste del tuo linguaggio naturale, controlla eventuali limiti o requisiti e crea piani dettagliati per aiutarti a raggiungere i tuoi obiettivi. A differenza dei semplici sistemi di domande e risposte, può regolare i suoi piani man mano che le cose cambiano, e può tornare indietro e provare diversi approcci se necessario. I piani creati vengono visualizzati nell’interfaccia di conversazione dell’Assistente di intelligenza artificiale, in modo da poter vedere e seguire il processo, nonché intervenire se necessario.

### Agenti Adobe Experience Platform {#agents}

| Agente | Dettagli | Applicazioni supportate |
| --- | --- | --- |
| [Audience Agent](audience.md) | Audience Agent consente di visualizzare informazioni approfondite sui tipi di pubblico, tra cui il rilevamento di modifiche significative nelle dimensioni del pubblico, il rilevamento di tipi di pubblico duplicati, l’esplorazione dell’inventario dei tipi di pubblico e il recupero delle dimensioni dei tipi di pubblico. | <ul><li>Real-Time CDP</li><li>Adobe Journey Optimizer</li></ul> |
| [Data Insights Agent](https://experienceleague.adobe.com/it/docs/analytics-platform/using/cja-overview/cja-b2c-overview/data-analysis-ai) | Data Insights Agent, accessibile dall’assistente di intelligenza artificiale in Customer Journey Analytics, è un agente di conversazione di intelligenza artificiale generativo che risponde in modo rapido ed efficiente alle domande sui tuoi dati. Crea visualizzazioni rilevanti in Analysis Workspace utilizzando i componenti della visualizzazione dati e utilizzando i dati effettivi. | Customer Journey Analytics |
| Agente di sperimentazione | L’agente di sperimentazione aiuta i team ad apprendere più rapidamente analizzando i risultati dell’esperimento, prevedendo l’impatto e proponendo nuovi esperimenti. Centralizza gli esperimenti passati e attivi in modo da poter sviluppare ciò che hai già imparato, individuare le lacune e assegnare priorità a ciò che verrà testato successivamente. | Adobe Journey Optimizer Experimentation Accelerator |
| [Journey Agent](./ajo-agent-analyze.md) | Journey Agent consente agli utenti di Adobe Journey Optimizer di creare, analizzare e ottimizzare i percorsi utilizzando un&#39;interfaccia in linguaggio naturale. Con Journey Agent, puoi creare rapidamente percorsi, rilevare e risolvere conflitti di pianificazione o di pubblico, analizzare le prestazioni e i punti di abbandono e identificare percorsi dalle prestazioni migliori da replicare per le campagne future. Consente di prendere decisioni basate sui dati, migliorare il coinvolgimento dei clienti e semplificare l’orchestrazione dei percorsi. | Adobe Journey Optimizer |
| [Agente di supporto del prodotto](https://experienceleague.adobe.com/it/docs/experience-platform/ai-assistant/new-features/customer-support) | Product Support Agent è una funzionalità self-service di debug e risoluzione dei problemi che consente di risolvere i problemi relativi alle funzioni e alle applicazioni di Adobe Experience Platform senza uscire dai flussi di lavoro. Gli amministratori del supporto possono creare ticket di assistenza clienti con il contesto delle interazioni dell’Assistente IA e controllare gli aggiornamenti dei ticket tramite l’Assistente IA. | <ul><li>Adobe Experience Platform</li><li>Real-Time CDP</li><li>Adobe Journey Optimizer</li><li>Adobe Journey Optimizer B2B edition</li><li>Customer Journey Analytics</li><li>Adobe Experience Manager</li></ul> |

### Knowledge base {#knowledge-base}

La knowledge base fornisce agli agenti un accesso sicuro alle informazioni aziendali dei clienti tramite origini dati strutturate e non strutturate, inclusa la documentazione di Adobe, i metadati dei clienti su oggetti aziendali e i dati di analisi.

## Accesso {#access}

Le richieste di AI Assistant vengono autenticate utilizzando i servizi di Adobe Identity Management. Le autorizzazioni vengono applicate dal controllo di accesso di Adobe Experience Platform e dal controllo di accesso di Customer Journey Analytics.

Per accedere all’interfaccia conversazionale dell’Assistente AI e utilizzare uno o più agenti Experience Platform, l’amministratore Adobe deve concedere le autorizzazioni pertinenti nell’interfaccia utente Autorizzazioni o in Adobe Admin Console:

* **Real-Time CDP** e **Adobe Journey Optimizer**: l&#39;amministratore deve concedere l&#39;autorizzazione **Abilita Assistente AI** per consentirti di accedere all&#39;Assistente AI. L&#39;amministratore deve inoltre concedere le autorizzazioni **Visualizza informazioni operative** per consentirti di porre domande su informazioni operative nell&#39;Assistente AI. Entrambe le autorizzazioni sono impostate dall’amministratore nell’interfaccia utente delle autorizzazioni.

* **Customer Journey Analytics**: l&#39;amministratore deve concedere l&#39;autorizzazione per accedere all&#39;Assistente di intelligenza artificiale tramite [Customer Journey Analytics Access Control](https://experienceleague.adobe.com/it/docs/analytics-platform/using/technotes/access-control). Questo consente di porre domande sulla conoscenza del prodotto e sulle informazioni sui dati.

>[!NOTE]
>
>Le domande relative agli approfondimenti operativi non sono disponibili per Customer Journey Analytics, pertanto non si applicano autorizzazioni aggiuntive.

* **Adobe Experience Manager**: l&#39;amministratore deve concedere l&#39;autorizzazione per accedere all&#39;Assistente di intelligenza artificiale tramite [Adobe Admin Console](https://helpx.adobe.com/it/enterprise/using/admin-console.html).


