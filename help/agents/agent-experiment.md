---
title: Experimentation Agent
description: Learn how to use Experimentation Agent
TQID: https://experienceleague.adobe.com/ARh16ylmUDrp---g8KuYNyewIv54IQ53pxoE2g700o0
product_v2: id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: f8a45b24-4be7-4f1b-909b-60d06b483a20id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: bcc5edb5-84c3-4940-9f84-ed88b6c16274id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: dd7883d8eccab3b0f006d55a850248e1c347d7e7
workflow-type: tm+mt
source-wordcount: 555
ht-degree: 4%

---

# Experimentation Agent

>[!AVAILABILITY]
>
>The Experimentation Agent is available to all customers who have purchased the paid license of Journey Optimizer Experimentation Accelerator and integrates seamlessly with either Adobe Target or Adobe Journey Optimizer.
>
>[Learn more on Journey Optimizer Experimentation Accelerator](https://experienceleague.adobe.com/it/docs/experimentation-accelerator/using/overview)

## Panoramica

The **Experimentation Agent** is an AI-powered tool that modernizes how you can run and manage digital experiments across websites, emails, push messages, and applications. Built on Adobe Experience Platform AI platform and experimentation tools, the **Experimentation Agent** helps you run experiments more efficiently, organize business goals, and generate actionable insights, highlighting what worked, what did not, and where to experiment next.

The following permissions in order to fully use the Experimentation Agent features.

* **View Experiments**: This permission lets you use the Experimentation Agent to view insights into the experiment directly in AI Assistant.

* **Manage Experiment Metada**: This permission lets you use the Experimentation Agent to create new experiments directly in AI Assistant.

➡️ [Learn more in Journey Optimizer Experimentation Accelerator documentation](https://experienceleague.adobe.com/en/docs/experimentation-accelerator/using/get-started/experiment-accelerator-access)

As part of Experimentation Accelerator feature, the Agent delivers:

* **Performance**: a clear view of what happened in the experiment

* **Insights**: an explanation of why the results occurred

* **Opportunities**: guidance on the next actions to take

![Sample for Experimentation Agent](./images/experiment/experiment-agent.png)

## Casi d’uso

The Experimentation Agent enhances each phase of the experimentation workflow by analyzing results, interpreting content, and suggesting next steps.

Its capabilities can be grouped into five key functions:

* **Experiment Summarization**

  Provide a clear, non-technical overview of experiment results for stakeholders.

* **Content Analysis**

  Examine the messaging or creative elements of treatments to understand why certain ones outperformed others.

* **Attribute Identification**

  Categorize treatments by their key attributes, e.g., themes, tones, formats, and connect those attributes to conversion outcomes.

* **Generazione consigli**

  Suggerisci nuovi trattamenti o aggiustamenti da testare, in base alle informazioni provenienti da esperimenti precedenti.

* **Opportunità**

  Identificare aree più ampie o nuovi angoli di sperimentazione per scoprire il potenziale non sfruttato.

## Funzioni nell&#39;ambito e fuori dall&#39;ambito

### **Rilevanti per l’ambito**

Sono attualmente supportate le seguenti funzionalità:

* Prestazioni
* Approfondimenti
* Opportunità

### **Non rilevanti per l’ambito**

Attualmente, le seguenti funzonalità non sono supportate:

* Creazione o modifica di esperimenti
* Utilizzo di più metriche per la generazione di rapporti sui casi d’uso

## Prompt di esempio

Di seguito è riportato un elenco di esempi di prompt che consentono di iniziare a utilizzare l’agente di sperimentazione:

### Domande generali

| Prompt |
|-|
| Quali esperimenti sono in esecuzione? |
| Quali esperimenti sono in esecuzione per `<campaign name>`? |
| Quali esperimenti sono iniziati nell&#39;ultimo mese? |
| Quanti esperimenti sono terminati l&#39;anno scorso? |
| Quali esperimenti sono attualmente in pausa/interrotti/ecc? |
| Quali pattern comuni stanno emergendo dai test recenti? |
| Qual è la durata media degli esperimenti nell&#39;ultimo trimestre? |

### Domande sulle prestazioni

| Prompt |
|-|
| Per il mio `<experiment name>`, quale trattamento sta conducendo? |
| Qual è l&#39;incremento di `<experiment name>`? |
| Quali esperimenti hanno avuto risultati statisticamente significativi? |
| Quali esperimenti avevano il tasso di conversione migliore? |

### Domande approfondite

| Prompt |
|-|
| Cosa è il test `<experiment name>`? ? |
| Cosa abbiamo imparato da `<experiment name>`? |
| Puoi dirmi perché ha vinto il trattamento A? |
| Quali temi hanno tendenza nelle varianti vincenti? |
| Quali pattern comuni stanno emergendo dai test recenti? |
| Si è verificato qualcosa di imprevisto in `<experiment name>`? |

### Domande sulle opportunità

| Prompt |
|-|
| Cosa consiglia di fare dopo questo esperimento? |
| È possibile migliorare `<experiment name>`? |
| Quali opportunità sono diventate più chiare dopo `<experiment name>`? |
| Cosa posso testare per dimostrare l&#39;ipotesi di `<experiment name>`? |
| Quali casi di utilizzo aggiuntivi devo implementare? |
