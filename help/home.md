---
title: IA nelle applicazioni Experience Cloud
description: Scopri come le applicazioni Experience Cloud utilizzano l’IA generativa (GenAI), l’Assistente IA e l’IA agentica.
TQID: https://experienceleague.adobe.com/heALjEZbowNaygG24oOM2HSlHa9oYVI5ViUNZDr19Ds
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: f8a45b24-4be7-4f1b-909b-60d06b483a20
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adeb
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: dd7883d8eccab3b0f006d55a850248e1c347d7e7
workflow-type: tm+mt
source-wordcount: 846
ht-degree: 17%

---

# IA in Experience Cloud

Welcome to the comprehensive guide for AI capabilities across Adobe Experience Cloud applications. This documentation covers how generative AI, AI Assistant, and Adobe agents are integrated into your Experience Cloud workflows to accelerate productivity and enhance decision-making.

## What&#39;s included in this guide

### Assistente IA

[AI Assistant](./ai-assistant/ai-assistant-ui.md) is an intelligent conversational, generative AI tool that will boost productivity and redefine work in Adobe Experience Platform-based Applications. Users can gain product knowledge, troubleshoot problems, and find operational insights through natural language prompts. You can also use AI Assistant to access Adobe Experience Platform Agents and other AI capabilities.

**Key features:**

- **Conversational Interface**: You can choose between a full-screen and a rail view interface to suit your workflow preferences.
- **Discovery Prompts**: AI Assistant provides pre-configured prompts that are organized by categories such as Learn, Analyze, and Optimize.
- **Context Setting**: You are able to configure the application, sandbox, and dataview settings to receive responses that are tailored to your needs.
- **Data Visualization**: The tool delivers interactive charts and graphs, enabling you to gain insights from your data.
- **Response Verification**: All responses include source citations, explanations of AI reasoning, and mechanisms for providing feedback.


### Agent Orchestrator

[Adobe Experience Platform Agent Orchestrator](./agents/agent-orchestrator.md) is the new agentic layer in Adobe Experience Platform. Progettato per sfruttare la ricca disponibilità di dati e le conoscenze della clientela della piattaforma, Agent Orchestrator di Experience Platform potenzia le informazioni e il ragionamento alla base degli Agenti esperti di Adobe Experience Platform appositamente creati, consentendo loro di eseguire complesse attività decisionali e di risoluzione dei problemi in modo rapido e su larga scala, sempre con intervento umano. Quando poni domande o richiedi assistenza tramite il linguaggio naturale in un’interfaccia conversazionale come l’Assistente IA, Agent Orchestrator richiama automaticamente ad agenti specializzati per ottenere le risposte giuste. Agent Orchestrator ricorda la cronologia delle conversazioni consentendoti di fare riferimento alle domande precedenti in modo naturale, senza dover ripetere il contesto, e combina gli insight provenienti da più agenti per fornire risposte chiare e unificate.

**Core components:**

- **Reasoning Engine**: Creates step-by-step plans and adjusts approaches as needed
- **Specialized Agents**: Purpose-built agents for specific tasks and domains
- **Knowledge Base**: Secure access to business intelligence and documentation

### Specialized Agents

#### Agente Audience

The Audience Agent provides insights about audiences including:

- Detecting significant audience size changes.
- Identifying duplicate audiences.
- Exploring audience inventory.
- Retrieving audience sizes.

Read the [Audience Agent documentation](./agents/audience.md) for more information.

#### Data Insights Agent

Disponibile in Customer Journey Analytics, il Data Insights Agent:

- Risponde a domande sui dati utilizzando il linguaggio naturale.
- Genera visualizzazioni rilevanti in Analysis Workspace.
- Utilizza componenti dalla visualizzazione dati e dati effettivi.

#### Agente analisi percorso

L’agente di analisi del Percorso consente agli utenti di Adobe Journey Optimizer di:

- Analizzare e ottimizzare i percorsi utilizzando il linguaggio naturale.
- Rileva e risolvi i conflitti di pianificazione o pubblico.
- Analizzare le prestazioni e i punti di rilascio.

Per ulteriori informazioni, leggere la [documentazione di Journey Agent](./agents/ajo-agent.md).

#### Agente di supporto prodotto

Utilizzare il Product Support Agent per il debug self-service e la risoluzione dei problemi:

- Risolvere i problemi relativi alle funzioni di Adobe Experience Platform senza uscire dai flussi di lavoro.
- Crea ticket di supporto con il contesto dalle interazioni dell’Assistente IA.
- Controlla gli aggiornamenti dei ticket tramite l’Assistente AI.

Per ulteriori informazioni, leggere la [documentazione dell&#39;agente di supporto tecnico](./agents/product-support.md).

<!--
#### Adobe Marketing Agent for [!DNL Microsoft 365 Copilot]

Use the Adobe Marketing Agent for [!DNL Microsoft 365 Copilot] to retrieve marketing insights from Experience Platform in [!DNL Microsoft 365] apps like [!DNL Teams], [!DNL Word], [!DNL Powerpoint], and [!DNL Excel]. With this agent, you can:

- Make faster, data-driven marketing decisions.
- Reduce time spent switching between tools.
- Simplify access to audience and journey insights across teams.

Read the [Adobe Marketing Agent documentation](./agents/ama-ms.md) for more information.
-->

## Guida introduttiva

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
