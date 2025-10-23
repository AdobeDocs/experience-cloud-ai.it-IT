---
title: Adobe Experience Platform Agent Orchestrator
description: Informazioni su Adobe Experience Platform Agent Orchestrator.
source-git-commit: a19c891d1a17c9112aff3d9a52daa94ad162a553
workflow-type: tm+mt
source-wordcount: '945'
ht-degree: 11%

---

# Adobe Experience Platform Agent Orchestrator

Agent Orchestrator di Adobe Experience Platform è il nuovo livello di agente in Adobe Experience Platform. Progettata per sfruttare i dati avanzati e le conoscenze dei clienti di Experience Platform, Experience Platform Agent Orchestrator potenzia l’intelligenza e il ragionamento alla base degli esperti Adobe Experience Platform Agent appositamente creati, consentendo loro di eseguire attività complesse di processo decisionale e risoluzione dei problemi in modo rapido e su larga scala, il tutto con la supervisione umana. Quando poni domande o richiedi assistenza tramite il linguaggio naturale in un’interfaccia conversazionale come l’Assistente IA, Agent Orchestrator richiama automaticamente ad agenti specializzati per ottenere le risposte giuste. Agent Orchestrator ricorda la cronologia delle conversazioni e consente di basarsi sulle domande precedenti in modo naturale, senza dover ripetere il contesto, e combina le informazioni provenienti da più agenti per fornire risposte chiare e unificate.

Puoi completare flussi di lavoro end-to-end complessi tramite un’interfaccia di conversazione intuitiva senza dover sapere quali agenti lavorano dietro le quinte. Il sistema comprende i tuoi obiettivi, crea piani dettagliati e regola il suo approccio in base alle tue esigenze. All’interno della conversazione in AI Assistant, puoi esplorare il pannello di ragionamento di Agent Orchestrator per vedere il processo di pensiero dettagliato e capire meglio come vengono gestite le richieste.

>[!SLIDE](agent-orchestrator-overview)

Leggi questo documento per scoprire di più su Agent Orchestrator.

## Componenti di Agent Orchestrator {#components}

Agent Orchestrator è costituito da diversi componenti chiave, tra cui l’interfaccia di conversazione dell’Assistente di intelligenza artificiale, un motore di ragionamento per il processo decisionale e la pianificazione, agenti Adobe Experience Platform specializzati e una knowledge base che fornisce l’accesso alle informazioni rilevanti.

![Architettura di marketing di Agent Orchestrator.](./images/agent-orchestrator/agentic-architecture.png)

### Interfaccia conversazionale dell’Assistente IA {#ai-assistant}

AI Assistant è un’esperienza di conversazione intelligente e in linguaggio naturale che consente ai professionisti che utilizzano applicazioni Experience Cloud abilitate di sfruttare le funzionalità GenAI e Agentic AI, la cui ampiezza dipende dalle applicazioni Experience Cloud concesse in licenza dai clienti. Per sbloccare l&#39;accesso, leggere [la guida all&#39;accesso all&#39;Assistente AI](https://experienceleague.adobe.com/it/docs/experience-platform/ai-assistant/access).

Per ulteriori informazioni, consulta la [Guida all’interfaccia utente dell’Assistente IA](../ai-assistant/ai-assistant-ui.md).

### Motore di ragionamento {#reasoning-engine}

Il motore di ragionamento interpreta i tuoi obiettivi in base alle richieste del tuo linguaggio naturale, controlla eventuali limiti o requisiti e crea piani dettagliati per aiutarti a raggiungere i tuoi obiettivi. A differenza dei semplici sistemi di domande e risposte, può regolare i suoi piani man mano che le cose cambiano, e può tornare indietro e provare diversi approcci se necessario. I piani creati vengono visualizzati nell’interfaccia di conversazione dell’Assistente di intelligenza artificiale, in modo da poter vedere e seguire il processo, nonché intervenire se necessario.

### Agenti Adobe Experience Platform {#agents}

Gli agenti Adobe Experience Platform sono un raggruppamento appositamente creato di agenti IA esperti nella distribuzione di processi comuni tra i domini di esperienza del cliente. Di seguito è riportato l’elenco degli agenti Adobe Experience Platform attualmente disponibili nelle applicazioni Experience Cloud:

| Agente | Dettagli | Applicazioni supportate |
| --- | --- | --- |
| [Audience Agent](audience.md) | Audience Agent consente di visualizzare informazioni approfondite sui tipi di pubblico, tra cui il rilevamento di modifiche significative nelle dimensioni del pubblico, il rilevamento di tipi di pubblico duplicati, l’esplorazione dell’inventario dei tipi di pubblico e il recupero delle dimensioni dei tipi di pubblico. | <ul><li>Real-Time CDP</li><li>Adobe Journey Optimizer</li></ul> |
| [Data Insights Agent](https://experienceleague.adobe.com/it/docs/analytics-platform/using/cja-overview/cja-b2c-overview/data-analysis-ai) | Data Insights Agent, accessibile dall’assistente di intelligenza artificiale in Customer Journey Analytics, è un agente di conversazione di intelligenza artificiale generativo che risponde in modo rapido ed efficiente alle domande sui tuoi dati. Crea visualizzazioni rilevanti in Analysis Workspace utilizzando i componenti della visualizzazione dati e utilizzando i dati effettivi. | Customer Journey Analytics |
| [Agente di sperimentazione](./agent-experiment.md) | L’agente di sperimentazione aiuta i team ad apprendere più rapidamente analizzando i risultati dell’esperimento, prevedendo l’impatto e proponendo nuovi esperimenti. Centralizza gli esperimenti passati e attivi in modo da poter sviluppare ciò che hai già imparato, individuare le lacune e assegnare priorità a ciò che verrà testato successivamente. | Adobe Journey Optimizer Experimentation Accelerator |
| [Journey Agent](./ajo-agent-analyze.md) | Journey Agent consente agli utenti di Adobe Journey Optimizer di creare, analizzare e ottimizzare i percorsi utilizzando un&#39;interfaccia in linguaggio naturale. Con Journey Agent, puoi creare rapidamente percorsi, rilevare e risolvere conflitti di pianificazione o di pubblico, analizzare le prestazioni e i punti di abbandono e identificare percorsi dalle prestazioni migliori da replicare per le campagne future. Consente di prendere decisioni basate sui dati, migliorare il coinvolgimento dei clienti e semplificare l’orchestrazione dei percorsi. | Adobe Journey Optimizer |
| [Agente di supporto del prodotto](https://experienceleague.adobe.com/it/docs/experience-platform/ai-assistant/new-features/customer-support) | Product Support Agent è una funzionalità self-service di debug e risoluzione dei problemi che consente di risolvere i problemi relativi alle funzioni e alle applicazioni di Adobe Experience Platform senza uscire dai flussi di lavoro. Gli amministratori del supporto possono creare ticket di assistenza clienti con il contesto delle interazioni dell’Assistente IA e controllare gli aggiornamenti dei ticket tramite l’Assistente IA. | <ul><li>Adobe Experience Platform</li><li>Real-Time CDP</li><li>Adobe Journey Optimizer</li><li>Adobe Journey Optimizer B2B edition</li><li>Customer Journey Analytics</li><li>Adobe Experience Manager</li></ul> |

Per ulteriori informazioni sulla disponibilità degli agenti nelle applicazioni Experience Cloud, consulta la [IA per agenti nella documentazione di Experience Cloud](https://experienceleague.adobe.com/it/docs/core-services/interface/features/agentic-ai).

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

