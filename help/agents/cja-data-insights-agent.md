---
description: Scopri come visualizzare i dati con Data Insights Agent in Customer Journey Analytics
title: Visualizzare i dati con Data Insights Agent in Customer Journey Analytics
role: User, Admin
solution: Customer Journey Analytics
source-git-commit: c29bac7450d29eda617dd712d7d5f55a0a2ca481
workflow-type: tm+mt
source-wordcount: '2497'
ht-degree: 1%

---

# Visualizzare i dati con Data Insights Agent

>[!AVAILABILITY]
>
>Data Insights Agent è disponibile per i clienti idonei per un periodo limitato. L’accesso a Data Insights Agent terminerà il 28 febbraio 2026. Per continuare a utilizzare Data Insights Agent senza interruzioni, contatta il rappresentante del tuo account Adobe per ulteriori informazioni sulle licenze di Data Insights Agent.

Data Insights Agent, accessibile dall&#39;[Assistente AI](https://experienceleague.adobe.com/it/docs/analytics-platform/using/cja-overview/cja-b2c-overview/ai-assistant) in Customer Journey Analytics, è un agente di conversazione di IA generativa che risponde in modo rapido ed efficiente alle domande sui tuoi dati. Crea visualizzazioni rilevanti in Analysis Workspace utilizzando i componenti della visualizzazione dati e utilizzando i dati effettivi.

L’utilizzo di Data Insights Agent per rispondere a domande incentrate sui dati in Analysis Workspace consente di risparmiare innumerevoli ore che altrimenti trascorreresti manualmente creando visualizzazioni in Analysis Workspace e acquisendo familiarità con i componenti di visualizzazione dati.

![Data Insights Agent nell&#39;Assistente AI](images/cja-agent//cja-ai-asst-da.gif)

## Caratteristiche interne ed esterne all&#39;ambito

| Funzione | In ambito | Fuori ambito |
| --- | --- | --- |
| **Tipi di visualizzazione** | <ul><li>LINE</li><li>Multiriga</li><li>Tabella a forma libera</li><li>Barra</li><li>Anello</li><li>Numero di riepilogo</li></ul> | <ul><li>Flusso</li><li>Fallout</li><li>Tabella coorte</li><li>Superfici, Superfici sovrapposte</li><li>Barre sovrapposte</li><li>Punto elenco</li><li>Combinato</li><li>Istogramma</li><li>Barre orizzontali, barre orizzontali sovrapposte</li><li>Riepilogo delle metriche chiave</li><li>A dispersione</li><li>Variazione di riepilogo</li><li>Testo</li><li>Mappa ad albero</li><li>Venn</li><li>Analisi guidata: crescita attiva, tendenze di conversione, coinvolgimento, impatto sul primo utilizzo, frequenza, Funnel, crescita netta, impatto sul rilascio, mantenimento, tempistica, tendenze</li></ul> |
| **Azioni Workspace e funzionalità agente** | <ul><li>Creare e aggiornare visualizzazioni<p>Genera una tabella a forma libera e la relativa visualizzazione (ad esempio una linea, una barra, un anello e così via).<p>Ad esempio, *Qual è il profitto tra SKU da febbraio a maggio?*</p></li><li>Fai domande di follow-up<p>Rispondi a un prompt nel contesto da qualsiasi prompt precedente. Ad esempio:</p> <ul><li>Prompt 1: *Eventi di tendenza da marzo.*</li><li>Prompt 2: *Visualizza i dati da marzo ad aprile*</li></ul> </li><li>Rilevamento di prompt fuori ambito<p>Se si invia una richiesta che non rientra nell&#39;ambito, ad esempio *Esporta questo progetto*, Data Insights Agent risponde informando che la domanda non rientra nell&#39;ambito.</p></li></ul> | <ul><li>Condividi</li><li>Esporta</li><li>Scarica</li><li>Gestire le preferenze utente</li><li>Gestire la visualizzazione dati</li><li>App delle dashboard di Analytics</li><li>Attribuzione</li><li>Riepilogo o risposta in linea<p>Data Insights Agent non può rispondere in linea nella barra chat con una risposta di riepilogo di un prompt utente. Esempi di prompt non inclusi nell&#39;ambito: *Visualizza un riepilogo degli approfondimenti dell&#39;ultimo prompt* e *Visualizza un riepilogo degli elementi evidenziati dalla visualizzazione delle linee.*</p></li></ul> |
| **Domande chiarificatrici** | Se si pone una domanda a cui non è disponibile un contesto sufficiente per la risposta di Data Insights Agent o che è troppo generica, Data Insights Agent risponde con una domanda chiarificatrice o con opzioni suggerite. <p>Le seguenti domande chiarificatrici sono esempi di domande relative alle componenti:</p><ul><li>Metrica: *Quale metrica &quot;ricavi&quot; intendevi usare?*</li><li>Dimension: *Specificare su quale delle seguenti &quot;aree geografiche&quot; concentrare l&#39;attenzione.*</li><li>Segmento: *Quale segmento &quot;Account&quot; desideri applicare?*</li><li>Intervallo date: *Per &quot;ultimo mese&quot;, intendevi l&#39;ultimo mese completo o gli ultimi 30 giorni?*</li></ul><p>La seguente domanda chiarificatrice è un esempio di una domanda relativa agli elementi dimensionali:</p> <ul><li>Quale &quot;nome del negozio&quot; intendevi? Ad esempio, #5274 store, #2949 store e così via.</li></ul> | Le domande più chiare sono limitate ai componenti e agli elementi dimensionali. Data Insights Agent non è in grado di chiarire elementi quali visualizzazioni dati, visualizzazioni, granularità dei dati, confronto e ambito. Quando non è possibile utilizzare le domande di chiarimento, l’agente utilizza per impostazione predefinita ciò che ti stai chiedendo. Se restituisce una visualizzazione o una granularità dei dati impreviste, puoi porre una domanda di follow-up o regolare la visualizzazione e i dati. |
| **Verificabilità e correttezza dei dati** | La verificabilità e la correttezza dei dati possono essere confermate visualizzando la tabella a forma libera e la visualizzazione dei dati generate. <p>Ad esempio, se chiedi a Data Insights Agent di *Trend ordini del mese scorso*, puoi confermare che la metrica corretta (&quot;ordini&quot;) e l&#39;intervallo di date (&quot;ultimo mese&quot;) siano stati selezionati nel pannello, nella visualizzazione dati e nella tabella a forma libera appena generati. | Data Insights Agent non risponde informando l’utente su quali componenti o visualizzazioni sono stati aggiunti.</p> |
| **Meccanismi di feedback** | <ul><li>Miniature in alto</li><li>Miniature in basso</li><li>Contrassegno</li></ul> |  |


## Gestire l’accesso a Data Insights Agent {#manage-access}

<!-- markdownlint-disable MD034 -->

>[!CONTEXTUALHELP]
>id="cja-enable-data-insights-data-view"
>title="Abilita per Data Insights Agent"
>abstract="Questa opzione abilita la visualizzazione dati per l’utilizzo con Data Insights Agent. Data Insights Agent è un agente di conversazione di intelligenza artificiale generativo accessibile dall’Assistente di intelligenza artificiale in Customer Journey Analytics. Consente di analizzare rapidamente i dati con messaggi di testo. Crea visualizzazioni rilevanti in Analysis Workspace utilizzando i componenti della visualizzazione dati e utilizzando i dati effettivi."

<!-- markdownlint-enable MD034 -->

I seguenti parametri regolano l’accesso a Data Insights Agent in Customer Journey Analytics:

* **Accesso alla soluzione**: Data Insights Agent è disponibile per tutti i clienti Customer Journey Analytics come parte di un programma di accesso limitato fino al 30 novembre 2025. Non è disponibile in Adobe Analytics.

* **Accesso contrattuale**: se non sei in grado di utilizzare Data Insights Agent nell&#39;Assistente AI, contatta l&#39;amministratore della tua organizzazione o il team dell&#39;account Adobe. Prima che la tua organizzazione possa utilizzare Data Insights Agent, devi accettare alcuni termini legali relativi all’intelligenza artificiale generativa.

* **Autorizzazioni**: per consentire agli utenti di accedere a Data Insights Agent, è necessario concedere le autorizzazioni necessarie in [!UICONTROL Adobe Admin Console].

  Per concedere le autorizzazioni, un [amministratore del profilo di prodotto](https://helpx.adobe.com/it/enterprise/using/manage-product-profiles.html) deve completare i seguenti passaggi in [!UICONTROL Admin Console]:
   1. In **[!UICONTROL Admin Console]**, seleziona la scheda **[!UICONTROL Prodotti]** per visualizzare la pagina **[!UICONTROL Tutti i prodotti e i servizi]**.
   1. Seleziona **[!UICONTROL Customer Journey Analytics]**.
   1. Nella scheda **[!UICONTROL Profili di prodotto]**, selezionare il titolo del profilo di prodotto per il quale si desidera fornire l&#39;accesso all&#39;[!UICONTROL Assistente AI: Conoscenza del prodotto].
   1. Nel profilo di prodotto specifico, seleziona la scheda **[!UICONTROL Autorizzazioni]**.

      ![Scheda Autorizzazioni in Admin Console](images/cja-agent/ai-assistant-permissions-tab.png)

   1. Nella riga **[!UICONTROL Strumenti di reporting]** nella tabella fornita, seleziona l&#39;icona di modifica ![Modifica](images/cja-agent/Edit.svg).
   1. Scorri fino a o cerca **[!UICONTROL Assistente AI: conoscenza del prodotto]**, quindi seleziona l&#39;icona più (![AddCircle](images/cja-agent/AddCircle.svg)) accanto a questa autorizzazione.
   1. Scorri fino a o cerca **[!UICONTROL Data Insights Agent]**, quindi seleziona l&#39;icona più (![AddCircle](images/cja-agent/AddCircle.svg)) accanto a questa autorizzazione.

      L&#39;autorizzazione **[!UICONTROL AI Assistant: Product Knowledge]** e l&#39;autorizzazione **[!UICONTROL Data Insights Agent]** sono state aggiunte alla colonna **[!UICONTROL Included permission items]**.

      ![Aggiungi autorizzazione](images/cja-agent/ai-assistant-permissions.png).

   1. Seleziona **[!UICONTROL Salva]** per salvare le autorizzazioni.

  Per ulteriori informazioni sul controllo di accesso, vedere [Controllo di accesso](https://experienceleague.adobe.com/it/docs/analytics-platform/using/technotes/access-control#access-control).

* **Accesso alla visualizzazione dati**: le visualizzazioni dati devono essere abilitate per Data Insights Agent.

  >[!IMPORTANT]
  >
  >Quando abiliti le visualizzazioni dati, tieni presente quanto segue:
  >* Puoi abilitare un massimo di 50 visualizzazioni dati per organizzazione IMS. Se abiliti più di 50 visualizzazioni dati in tutti i profili di prodotto per una determinata organizzazione, Data Insights Agent utilizzerà le 50 visualizzazioni dati più utilizzate.
  >* Data Insights Agent può fare riferimento alle visualizzazioni dati incluse nello stesso giorno in cui vengono abilitate.

  Per abilitare le visualizzazioni dati per Data Insights Agent:

   1. In Customer Journey Analytics, seleziona **[!UICONTROL Gestione dati]** > **[!UICONTROL Visualizzazioni dati]**.

   1. Selezionare una o più visualizzazioni dati da abilitare per Data Insights Agent, quindi selezionare **[!UICONTROL Abilita per Data Insights Agent]**.

      ![Abilita visualizzazioni dati per Data Insights Agent](images/cja-agent/data-view-enable-dia.png)

  Per visualizzare il numero di visualizzazioni dati abilitate per Data Insights Agent nell’organizzazione IMS:

   1. In Customer Journey Analytics, seleziona **[!UICONTROL Gestione dati]** > **[!UICONTROL Visualizzazioni dati]**.

   1. Seleziona l&#39;icona info nella parte superiore della colonna **[!UICONTROL Data Insights Agent]**.

      ![Icona info Data Insights Agent](images/cja-agent/data-insights-agent-tooltip.png)

## Accedere a Data Insights Agent nell’Assistente AI

1. Vai a [experience.adobe.com](https://experience.adobe.com/) e accedi con il tuo Adobe ID.

2. Seleziona **Customer Journey Analytics** dalla Home di Experience Cloud.

3. Seleziona **[!UICONTROL Progetto vuoto]** nel banner nella parte superiore della pagina dei progetti per aprire un nuovo progetto vuoto.

4. Verificare che la visualizzazione dati selezionata per il pannello sia abilitata per l&#39;utilizzo con Data Insights Agent, come descritto in [Gestione dell&#39;accesso a Data Insights Agent in Customer Journey Analytics](#manage-access-to-data-insights-agent-in-customer-journey-analytics).

5. Seleziona l’icona della chat dell’Assistente AI nell’area in alto a destra della pagina.

   Se l’icona della chat non è visibile, contatta l’amministratore in modo che possa abilitare le seguenti funzioni in Admin Console:

   * Strumenti di reporting: **[!UICONTROL Assistente AI: Conoscenza del prodotto]**

   * Strumenti visualizzazione dati: **[!UICONTROL Data Insights Agent]**

   Per ulteriori dettagli, vedere [Gestire l&#39;accesso a Data Insights Agent in Customer Journey Analytics](#manage-access-to-data-insights-agent-in-customer-journey-analytics).

   ![Icona Assistente IA](images/cja-agent/ai-asst-icon.png)

6. Nella finestra di dialogo **[!UICONTROL Chiedi informazioni su Customer Journey Analytics]** nella parte inferiore della pagina, fai una domanda sulla visualizzazione dei dati utilizzando Data Insights Agent.

   Per ulteriori informazioni, vedi gli esempi seguenti.

### Esempio 1

Ad esempio, supponiamo che tu sia interessato agli ordini ricevuti dalla tua azienda in luglio.

**Prompt:** Inserisci *&quot;Trend ordini in luglio.&quot;*

![prompt IA](images/cja-agent/ai-asst-prompt1.png)

**Risposta:** Data Insights Agent raccoglie informazioni approfondite esaminando i dati nella visualizzazione dati, incluse le metriche e i componenti. Traduce il prompt nelle dimensioni e nelle metriche corrette all’interno dell’intervallo di dati.

Come puoi vedere, ha generato automaticamente un grafico a linee e una tabella a forma libera per mostrare gli ordini di luglio.

![Risposta alla richiesta - grafico a linee e tabella a forma libera](images/cja-agent/ai-asst-result.png)

### Esempio 2

Ora vuoi vedere come si confrontano i ricavi per regione.

**Prompt:** Nella finestra del prompt, immettere *&quot;Mostra ricavi per area&quot;*

**Risposta:** Data Insights Agent comprende in modo intelligente che per &quot;area geografica&quot; si intende &quot;area del cliente&quot;. Produce un grafico a barre che mostra al meglio i ricavi per area:

![Grafico a barre](images/cja-agent/ai-asst-result2.png)

### Esempio 3

Quindi, oltre a comprendere i ricavi per area, vuoi anche visualizzare i dati per i profitti per area. Invece di ripetere la richiesta precedente, puoi chiedere a Data Insights Agent di aggiornare la visualizzazione e la tabella a forma libera più recenti.

**Prompt:** Nella finestra del prompt, digitare *&quot;Aggiungi profitto.&quot;*

**Risposta:** Il grafico **[!UICONTROL Barre]** fornisce ancora la risposta più concisa, ma la metrica di profitto è stata aggiunta come colonna nella tabella a forma libera:

![Grafico a barre](images/cja-agent/ai-asst-result4.png)

### Esempio 4

Infine, esaminiamo i ricavi per categoria di prodotto.

**Prompt:** Nella finestra del prompt, immettere *&quot;Proporzione di ricavi per categoria di prodotto.&quot;*

**Risposta:** Anche in questo caso, Data Insights Agent sceglie la visualizzazione più appropriata, in questo caso **[!UICONTROL Anello]**, per rispondere alla domanda.

![Anello](images/cja-agent/ai-asst-result3.png)

## Accedere a Data Insights Agent nelle applicazioni Experience Cloud

Adobe Experience Platform Agent Orchestrator consente di accedere alle funzionalità di Data Insights Agent in più applicazioni Adobe Experience Cloud, ad esempio Adobe Journey Optimizer e Real-Time CDP.

Agent Orchestrator interpreta la richiesta, determina quali agenti specializzati sono necessari e li orchestra per fornire la risposta giusta. Tiene traccia del contesto nelle interazioni a più turni, in modo da poter sfruttare naturalmente le query precedenti.

Per ulteriori informazioni, vedere [Adobe Experience Platform Agent Orchestrator](/help/agents/agent-orchestrator.md).

## Esempio di prompt di visualizzazione dati

Di seguito sono riportati alcuni esempi di prompt comuni e delle visualizzazioni utilizzate da Data Insights Agent per rispondere a tali prompt.

| Esempio di prompt | Visualizzazione prevista |
| --- | --- |
| Mostra profitti in [Mese] | LINE<p>La richiesta di una tendenza o di una metrica entro un determinato intervallo di tempo per impostazione predefinita restituisce una visualizzazione a linee. |
| Andamento ordini in [Mese] | LINE |
| Mostra ricavi per area geografica in [Mese] | Barra |
| Quota di ricavi per categoria di prodotto | Anello |
| Ordini per giorno della settimana, da gennaio a maggio | Barra |
| Mostra ordini per genere, da marzo a giugno | Barra |
| Qual è il profitto tra SKU da febbraio a maggio | Barra |
| Ricavi per nome archivio in [Mese] | Barra |
| Quali sono stati i miei 10 SKU principali in base al profitto in [Mese]? | Barra |
| Percentuale di acquisti per mese dell&#39;anno | Anello |
| Profitto totale in [Mese] | Numero di riepilogo<p>Se si richiede il &quot;totale&quot; di una metrica in un determinato intervallo di tempo, viene restituita una visualizzazione del numero di riepilogo. |


## Best practice per la richiesta di informazioni

Data Insights Agent elabora il contesto fornito da ogni richiesta dell’utente e tenta di rispondere in modo intelligente con la visualizzazione e i componenti più appropriati in una tabella a forma libera.

Le risposte possono variare in base alle parole e alle frasi specifiche utilizzate nel prompt, e lievi modifiche nella lingua possono portare a risultati diversi.

Per ottenere i migliori risultati, considera le seguenti linee guida:

* **Specificare:** Includere termini esatti per limitare la risposta. Di seguito è riportato un esempio di un prompt specifico: &quot;Vendite del mese scorso in California&quot;

* **Usa metriche, dimensioni e segmenti chiari:** L&#39;aggiunta di metriche specifiche (ad esempio &quot;Ricavi&quot;), dimensioni (ad esempio &quot;nome sito Web&quot;), segmenti (ad esempio &quot;utenti iPhone&quot;) e intervalli di date (ad esempio &quot;ultimi tre mesi&quot;) consente a Data Insights Agent di concentrarsi sui dati giusti.

* **Fai domande dirette:** La formulazione delle domande semplifica la fornitura da parte di Data Insights Agent di informazioni chiare e pertinenti. Di seguito è riportato un esempio di una domanda diretta in un prompt: &quot;Qual è il reddito medio per categoria di prodotto quest&#39;anno?&quot;

Rivedi la seguente tabella di termini e frasi di esempio che puoi utilizzare nei prompt con Data Insights Agent, insieme ai tipi di risposte che puoi aspettarti.

Questi esempi sono progettati per aiutarti a capire in che modo parole o strutture specifiche possono influenzare l’output dell’agente di Data Insight, garantendo informazioni più precise e preziose. Data Insights Agent utilizza un’intelligenza artificiale generativa, pertanto le visualizzazioni o i dati selezionati possono variare leggermente in base a prompt simili.

| Risultato desiderato | Termini e frasi di esempio |
| --- | --- |
| Visualizzazione Numero di riepilogo | <ul><li>Totale</li></ul> |
| Confronta componenti | <ul><li>Confronta</li><li>VS</li><li>Contrasto</li><li>Settimana per settimana</li><li>Su base mensile</li><li>Trimestre su trimestre</li><li>Anno su Anno</li></ul> |
| Visualizzazione ad anello | <ul><li>Proporzione</li><li>Quota di</li><li>Distribuzione</li><li>Percentuale</li><li>Contributo</li><li>Porzione</li><li>Parti</li></ul> |
| Visualizzazione Linee | <ul><li>Tendenza</li><li>[Metrica] in [Intervallo di tempo]</li></ul> |
| Visualizzazione a barre | <ul><li>[Metrica] da [Dimension]</li></ul> |

<!--

## Beta testing expectations and requested feedback

After posing each question, carefully review the assistant's provided answer. It's crucial to evaluate the generated visualizations comprehensively before providing feedback. 

Consider the following when evaluating a response from Data Insights Agent: 

* Chat rail response or template: Evaluate the textual response provided. Is the response appropriate given the context of your prompt? 

* Visualization/chart: Evaluate the visualization. Is it the appropriate or expected visualization for your question, or would you have expected a different visualization?  

* Freeform table: Evaluate the freeform table. Is the freeform table data correct? Is it breaking down data where requested? Are the applied segments those that you requested or expected? 

* Error Message / Out-of-Scope: If a generic error message is given stating the question is out of scope, provide feedback on whether you think the out-of-scope message is appropriate, given your prompt. Was your prompt actually in scope? 

**For every response, give a thumbs up or thumbs down, based on the response.**

Following the thumbs up or thumbs down selection, please make a selection for the relevant multi-select feedback boxes. If you want to provide additional feedback, add notes in the open text box.

## Questions and Contact

* Send questions and feedback in the Beta Slack channel: #data-insights-agent-in-cja-beta

-->


## Best practice di configurazione

Di seguito sono riportate le best practice per la configurazione di Customer Journey Analytics (visualizzazione dati, metriche calcolate, segmenti e altro ancora) per garantire che Data Insights Agent possa individuare i componenti corretti e restituire risposte più chiare senza dover richiedere ulteriori informazioni.

* **Bilanciare i componenti necessari**. Non aggiungere tutti i campi dei set di dati come metriche o componenti dimensione alla visualizzazione dati. In particolare, quelli che certamente non utilizzerai nell’analisi. D’altra parte, non limitarti strettamente ai campi che ritieni necessari per l’analisi. Una visualizzazione dati troppo limitata limita la flessibilità dell’analisi e la funzionalità Data Insights Agent.
* **Utilizza sempre nomi descrittivi**. Assicurati che tutti i campi definiti nella visualizzazione dati, come componente di metrica o di dimensione, abbiano un nome di componente descrittivo. Il processo di ridenominazione dei campi con un nome descrittivo è particolarmente importante per i campi dei set di dati del connettore di origine di Adobe Analytics. Questi campi hanno spesso nomi non descrittivi non identificabili, come `eVar41` o `prop25`.
* **Usare nomi distinti**. I nomi distinti sono particolarmente rilevanti quando utilizzi lo stesso campo sia come componente metrica che come componente dimensione nella visualizzazione dati. Oppure quando utilizzi un campo in più componenti dello stesso tipo (ad esempio in due metriche diverse), ciascuno con impostazioni di componenti diverse.
* **Utilizzare una convenzione per la denominazione dei componenti**. È possibile utilizzare una convenzione di denominazione dei componenti per raggruppare i componenti. Ad esempio, **[!UICONTROL Ordini | Prodotto]** e **[!UICONTROL Ordini | Il cliente]** è in grado di distinguere tra diverse metriche dell&#39;ordine che potrebbero esistere nei tuoi dati.
* **Utilizza il dizionario dati**. Aggiungi una descrizione e altri dati rilevanti per i componenti nel dizionario dati. L’agente di Data Insight attualmente non utilizza i tag description e tag del dizionario dati, ma potrebbe farlo in futuro.
* **Utilizzare le metriche calcolate approvate**. Concordare un processo per utilizzare solo metriche calcolate approvate come componenti nella visualizzazione dati ed evitare di utilizzare metriche calcolate sperimentali.
* **Condividi i segmenti richiesti**. Assicurati di condividere i segmenti e renderli visibili necessari per le richieste di Data Insights Agent.
* **Standardizzare i nomi dei componenti nelle visualizzazioni dati**. Se utilizzi gli stessi campi come componente in più visualizzazioni dati, assicurati di utilizzare un singolo nome descrittivo e un singolo identificatore per quel componente. Un singolo nome e identificatore consente a Data Insights Agent di cambiare visualizzazione dati senza perdere contesto.

>[!MORELIKETHIS]
>
>[Impostazioni dei componenti](https://experienceleague.adobe.com/it/docs/analytics-platform/using/cja-dataviews/component-settings/overview)
>[Dizionario dati](https://experienceleague.adobe.com/it/docs/analytics-platform/using/cja-components/data-dictionary/data-dictionary-overview)
>[Approva metrica calcolata](https://experienceleague.adobe.com/it/docs/analytics-platform/using/cja-components/cja-calcmetrics/cm-workflow/cm-approving)
>[Condividi segmenti](https://experienceleague.adobe.com/it/docs/analytics-platform/using/cja-components/segments/seg-share)
>
