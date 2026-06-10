---
title: Agente notifiche
description: Scopri come utilizzare l’agente di notifiche nell’Assistente all’intelligenza artificiale per riepilogare, interpretare e agire sulle notifiche aziendali di Adobe CX utilizzando il linguaggio naturale.
source-git-commit: d4254ada196055b869e6392b6d8cc2d4a037c4ad
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 1%

---

# Agente notifiche

L&#39;Agente notifiche aggiunge un livello di intelligenza artificiale conversazionale all&#39;interno di [Assistente IA](../ai-assistant/ai-assistant-ui.md) che è possibile utilizzare per riepilogare, interpretare e agire sulle notifiche utilizzando il linguaggio naturale, trasformando in tal modo un feed passivo in un assistente attivo. Invece di scansionare un lungo elenco, puoi passare da &quot;Ho 47 notifiche&quot; a &quot;2 hanno bisogno della mia approvazione entro venerdì, 3 set di dati hanno conflitti, il resto è FYI&quot; in un singolo scambio.

## Quali funzioni può eseguire l’agente di notifica

L’agente di notifica supporta le seguenti funzionalità:

| Funzionalità | Descrizione |
| --- | --- |
| **Riepiloghi e informazioni sulle notifiche** | Ottieni panoramiche concise delle tue notifiche, fai una chiara distinzione tra quelle che richiedono un’azione e quelle che sono solo informative e comprendi sia lo scopo di una notifica che il motivo per cui l’hai ricevuta. |
| **Azioni operative** | Intervenire direttamente sulle notifiche tramite conversazione, contrassegnandole come lette, note o impostare promemoria per le notifiche singole o raggruppate. |
| **Preferenze e impostazioni** | Attiva o disattiva i canali di notifica (e-mail, Slack, in-app) per soluzione e categoria, senza passare da Impostazioni. |
| **Navigazione e collegamenti diretti** | Passa direttamente da una notifica all’area del prodotto rilevante tramite collegamenti profondi. |
| **Collaboration e condivisione** | Condividi notifiche o invia annunci ai destinatari all’interno della stessa organizzazione. |

## Agente notifiche di accesso

Puoi accedere all’agente notifiche nei modi seguenti:

- **Dall&#39;Assistente AI**: aprire l&#39;Assistente AI e immettere eventuali prompt relativi alle notifiche.
- **Dalla libreria di prompt**: seleziona un prompt suggerito che soddisfi le tue esigenze.

## Prompt di esempio

Leggi le sezioni seguenti per esempi di prompt che puoi utilizzare con l’agente di notifica.

### Riepiloghi e informazioni

- &quot;Riepiloga le notifiche recenti.&quot;
- &quot;Quale delle mie notifiche ha bisogno della mia azione rispetto a cosa è solo FYI?&quot;

### Azioni

- &quot;Contrassegna tutte le notifiche non actionable come lette.&quot;
- &quot;Ricordami della notifica {NOTIFICATION_OF_INTEREST} tra un&#39;ora.&quot;

### Preferenze

- &quot;Abilita le notifiche Slack per Journey Optimizer.&quot;
- &quot;Cambia il riepilogo giornaliero a settimanale.&quot;

### Collaborazione

- &quot;Condividi questa notifica con {EMAIL_ADDRESS_OF_USER_IN_YOUR_ORG}.&quot;

## Best practice

Tieni presente i seguenti suggerimenti quando utilizzi l’agente di notifica:

- **Specificare**: assegnare un nome chiaro all&#39;app, alla notifica, alla categoria di notifica e al canale in modo che l&#39;agente possa agire sulla destinazione prevista.
- **Prompt catena**: è possibile richiedere un riepilogo, eseguire il completamento concentrandosi su una notifica specifica e quindi eseguire un&#39;azione, il tutto all&#39;interno di una singola conversazione.
- **Risposta alle domande chiarificatrici**: quando l&#39;agente richiede conferma sull&#39;app, sul canale o sulla notifica, assicurati di rispondere in modo che le modifiche vengano applicate correttamente.
