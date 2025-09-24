---
title: Privacy, sicurezza e governance nell’Assistente di IA
description: Scopri le procedure di privacy, sicurezza e governance per l’Assistente IA.
source-git-commit: fe4d2de03e34eccd2950f87b3c57ffbb5e1cf5e9
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---

# Privacy, sicurezza e governance nell’Assistente di IA

L’Assistente per l’intelligenza artificiale in Adobe Experience Platform è stato progettato con privacy, sicurezza e governance in primo piano.

Leggi questo documento per scoprire le funzionalità incentrate sulla fiducia dei clienti che puoi aspettarti dall’Assistente AI:

* Nessun dato personale viene utilizzato oggi da AI Assistant, anche a scopo di formazione.
* L’Assistente AI non è a conoscenza dei dati del consumatore.
* Tutti i criteri di [controllo dell&#39;accesso](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/home) esistenti verranno rispettati dall&#39;Assistente IA.

   * Eventuali nuovi criteri di controllo dell’accesso basati su attributi vengono rispecchiati in IA Assistant dopo un massimo di 24 ore&amp;ast;

* Per interagire con l&#39;Assistente AI è necessario disporre dell&#39;autorizzazione esplicita.

   * Puoi impostare le autorizzazioni in modo diverso per Experience Platform e Journey Optimizer utilizzando la [Interfaccia utente autorizzazioni](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/abac/permissions-ui/browse) e puoi utilizzare la [Admin Console](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/ui/browse) per assegnare le autorizzazioni per Customer Journey Analytics.
   * Le autorizzazioni sono granulari e l’amministratore della sandbox può configurare quali dei tuoi utenti possono porre diverse categorie di domande (domande basate sulla conoscenza del prodotto con l’Assistente AI o domande sulle informazioni operative).

* L&#39;Assistente AI è una funzione compatibile con HIPAA se utilizzata in combinazione con Adobe Experience Platform Healthcare Shield.
* È possibile visualizzare un registro delle interazioni precedenti con l’Assistente AI con un criterio di conservazione di 30 giorni.
* L’Assistente AI si basa sui dati specifici delle sandbox e sulla documentazione pubblica di Adobe quando si rispondono alle richieste degli utenti. I dati non sono condivisi tra sandbox diverse.
* I prompt forniti all&#39;Assistente IA non vengono condivisi con altri clienti.

&amp;ast; *Questo implica che se vengono aggiunte nuove etichette a campi e oggetti o vengono creati nuovi criteri, l’Assistente AI impiegherà fino a 24 ore per rispettarli. Durante queste 24 ore, gli utenti con accesso limitato di recente possono comunque accedere a tali campi e oggetti.*
