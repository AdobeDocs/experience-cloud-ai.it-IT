---
solution: Real-Time Customer Data Platform
title: Real-Time CDP MCP (Beta)
description: Scopri come collegare Adobe Real-Time CDP ai client MCP utilizzando il server MCP.
feature: Integrations
topic: Content Management, Artificial Intelligence
badge: label="Beta" type="Informative"
role: User, Developer
level: Beginner, Intermediate
source-git-commit: b2c93fd31bb72ebaf79aaa07aab68d39e63dc9b5
workflow-type: tm+mt
source-wordcount: '2634'
ht-degree: 0%

---

# Real-Time CDP MCP (Beta) {#rtcdp-mcp}

È possibile utilizzare l’integrazione MCP di Adobe Real-Time CDP per eseguire query su tipi di pubblico, destinazioni e stato di attivazione utilizzando prompt in linguaggio semplice, senza scrivere chiamate API o navigare tra le schermate dei prodotti. Questa integrazione è utile sia per i clienti Adobe Real-Time CDP che per i clienti Adobe Real-Time CDP B2B edition e offre un modo conversazionale per ispezionare i dati e i flussi di lavoro Real-Time CDP supportati da client compatibili con MCP. Leggi questa guida per scoprire come funziona l’integrazione, cosa puoi farci e come iniziare.

>[!AVAILABILITY]
>
>Real-Time CDP MCP è in Beta. La funzione e la documentazione sono soggette a modifiche. Il server MCP di Real-Time CDP è distribuito come **server di trasporto HTTP remoto** che gli utenti installano e configurano nei client MCP e nelle piattaforme app supportati (ad esempio, [!DNL Claude], [!DNL ChatGPT], [!DNL Claude Code], [!DNL Codex], [!DNL Cursor] o [!DNL VS Code]). L&#39;autenticazione viene gestita tramite un **flusso di accesso basato su browser**. Quando il client si connette per la prima volta al server, apre il browser predefinito in modo che tu possa accedere con le tue credenziali Adobe e autorizzare l&#39;accesso. Contatta il rappresentante Adobe per accedere a questo programma Beta.

## Beta, sicurezza e note legali {#mcp-notices}

**Avviso di documentazione di Beta:** questa documentazione riguarda una funzionalità di Beta e non costituisce documentazione finale. Il contenuto qui descritto si riferisce a una versione di Beta ed è soggetto a modifiche prima della disponibilità generale. Adobe non fornisce alcuna dichiarazione sulla completezza o sull’accuratezza di questa documentazione.

Utilizzando il server Adobe Real-Time CDP MCP (Beta) (&quot;Beta&quot;), l&#39;utente riconosce che il Beta è fornito **&quot;così com&#39;è&quot; senza alcuna garanzia**. Adobe non ha alcun obbligo di mantenere, correggere, aggiornare, modificare, modificare o supportare in altro modo Beta. Si consiglia di usare cautela e di non fare affidamento in alcun modo sul corretto funzionamento o sulle prestazioni di tale Beta e/o dei materiali di accompagnamento. Beta è considerata un&#39;informazione riservata di Adobe. Qualsiasi &quot;Feedback&quot; (informazioni relative a Beta, compresi, a titolo esemplificativo e non esaustivo, problemi o difetti riscontrati durante l’utilizzo di Beta, suggerimenti, miglioramenti e raccomandazioni) fornito dall’Utente a Adobe viene assegnato ad Adobe, inclusi tutti i diritti, i titoli e gli interessi relativi a tale Feedback.

>[!WARNING]
>
>Il Model Context Protocol (MCP) è uno standard open source emergente e può presentare rischi per la sicurezza o l&#39;affidabilità. Le integrazioni server MCP di Adobe e la relativa documentazione vengono fornite &quot;così come sono&quot;, senza garanzie di alcun tipo.
>
>La connessione di client o server MCP ai prodotti Adobe è una configurazione selezionata dal cliente. I clienti sono responsabili della valutazione della sicurezza e dell&#39;idoneità di qualsiasi integrazione MCP. Adobe non è responsabile dei problemi derivanti da configurazione errata, utilizzo errato di MCP, vulnerabilità in implementazioni di terze parti o azioni non intenzionali eseguite tramite flussi di lavoro abilitati per MCP.
>
>Per ridurre i rischi, Adobe incoraggia a testare le integrazioni in un ambiente sandbox prima di utilizzarle in modo produttivo e a rivedere e convalidare attentamente tutte le azioni e le risposte avviate da MCP prima di confermarle o di fare affidamento su di esse.

## Qual è il protocollo di contesto del modello? {#mcp-overview}

I team di marketing, dati e customer-experience si affidano sempre di più ad applicazioni basate su chat e a strumenti per sviluppatori, come Anthropic Claude, OpenAI ChatGPT, Cursor e Microsoft Copilot Studio, per semplificare il loro lavoro quotidiano. Queste applicazioni supportano **Model Context Protocol (MCP)**, uno standard aperto che consente alle applicazioni di esporre gli strumenti back-end a modelli LLM (Large Language Model) in modo uniforme.

Real-Time CDP ora fornisce un server MCP che mette in evidenza le operazioni di pubblico, destinazione e attivazione direttamente all&#39;interno di qualsiasi applicazione compatibile con MCP. Con l’integrazione MCP di Real-Time CDP, utenti tipo diversi possono collaborare intorno agli stessi dati di segmentazione e attivazione, senza scrivere query sulle API REST di Adobe Experience Platform o navigare su più schermate dell’interfaccia utente. I clienti possono descrivere il proprio intento conversazionalmente e consentire al LLM di richiamare gli strumenti MCP appropriati.

## Funzionalità principali {#mcp-capabilities}

Il server MCP di Real-Time CDP è una **superficie di monitoraggio e valutazione di sola lettura**. Espone le API di recupero per tipi di pubblico, destinazioni, origini, identità e risoluzione dei profili come risposte in linguaggio semplice all’interno dell’assistente AI, senza scrivere query o navigare tra le schermate dei prodotti. Non è possibile creare, modificare o eliminare dati tramite il server MCP.

>[!IMPORTANT]
>
>Tutti gli strumenti nel Beta corrente sono **di sola lettura**. Le operazioni di scrittura, tra cui la creazione, l’attivazione, l’aggiornamento o l’eliminazione di tipi di pubblico, destinazioni o flussi di dati, non sono supportate.

Il rilascio di Beta include i seguenti 18 strumenti:

| Strumento | Descrizione |
| --- | --- |
| `search_audiences` | Elenca e cerca i tipi di pubblico per nome, tipo di entità, stato del ciclo di vita, spazio dei nomi dell’identità o origine. |
| `preview_audience_membership` | Stimare la dimensione di un’espressione di segmento PQL o SDD prima di salvarla come pubblico. |
| `inspect_audience_evaluation_jobs` | Recupera i record del processo di valutazione del segmento per diagnosticare il motivo per cui un pubblico batch non viene aggiornato o per confermare la cronologia di valutazione recente. |
| `inspect_audience_export_jobs` | Recupera i record del processo di esportazione del pubblico per confermare le esportazioni completate o i dettagli dell’errore della superficie. |
| `search_destination_connectors` | Elencare i tipi di connettore di destinazione disponibili nella piattaforma (ad esempio [!DNL Amazon S3], [!DNL Google Ads], [!DNL Salesforce] CRM). |
| `search_destination_accounts` | Elenca account di destinazione autenticati: istanze configurate di un tipo di connettore di destinazione. |
| `search_destination_input_connections` | Recupera l’input lato Experience Platform di un flusso di destinazione: il pubblico o il set di dati da esportare. |
| `search_destination_output_connections` | Recupera l’endpoint esterno di un flusso di destinazione: percorso di destinazione, formato del file e configurazione di consegna. |
| `search_destination_flows` | Elenca e controlla i flussi di attivazione delle destinazioni configurati, compresi il loro stato, le mappature e la pianificazione. |
| `inspect_flow_runs` | Recupera la cronologia di esecuzione per i flussi di origine e di destinazione: stato, tempistica, conteggi dei record e dettagli degli errori per esecuzione. |
| `search_source_connectors` | Elencare i tipi di connettore di origine disponibili nella piattaforma. |
| `search_source_accounts` | Elenca account di origine autenticati: istanze configurate di un tipo di connettore di origine. |
| `search_source_input_connections` | Recupera il livello di selezione dei dati di un flusso sorgente, ovvero ciò che viene estratto da un account. |
| `search_source_output_connections` | Recupera la destinazione del set di dati di Experience Platform di un flusso di origine, dove arrivano i dati acquisiti. |
| `search_source_flows` | Elenca e controlla le pipeline di acquisizione di origine configurate, compresi il loro stato, le mappature e la pianificazione. |
| `search_identity_namespaces` | Elencare le definizioni degli spazi dei nomi delle identità nella sandbox, sia negli spazi dei nomi standard che personalizzati di Adobe. |
| `search_merge_policies` | Elenca i record dei criteri di unione che controllano il modo in cui i profili cliente in tempo reale vengono assemblati dai frammenti di profilo. |
| `search_organizations` | Elenca le organizzazioni Adobe accessibili all’utente autenticato. |

## Casi d’uso {#mcp-use-cases}

Il server MCP di Real-Time CDP è progettato per il monitoraggio e la valutazione **1&rbrace;.** Poiché il server funziona con gli ID piuttosto che con i nomi, un flusso di lavoro tipico inizia con un elenco: chiedi a Claude di mostrarti cosa è disponibile, scegli l&#39;elemento desiderato, quindi fai domande di follow-up utilizzando l&#39;ID che restituisce.

| Obiettivo | Esempio di prompt |
| --- | --- |
| **Elencare i tipi di pubblico** | &quot;Elenca i miei tipi di pubblico nella sandbox `prod`.&quot; |
| **Controllare un pubblico specifico** | &quot;Visualizza i dettagli e lo stato del ciclo di vita per l&#39;ID pubblico `abc123`.&quot; |
| **Diagnosticare un errore di valutazione** | &quot;Mostra i processi di valutazione più recenti e contrassegna eventuali errori.&quot; |
| **Controlla un processo di esportazione** | &quot;Elenca i processi di esportazione del pubblico recenti e mostrami lo stato di ciascuno di essi.&quot; |
| **Stimare la dimensione del pubblico** | &quot;Stimare la dimensione di questa espressione PQL prima di salvarla: `homeAddress.country = 'US'`.&quot; |
| **Elenca i tipi di connettore di destinazione** | &quot;Quali tipi di connettore di destinazione sono disponibili nella sandbox?&quot; |
| **Elenca account di destinazione configurati** | &quot;Elenca gli account di destinazione e il relativo stato di connessione.&quot; |
| **Elenca flussi di destinazione** | &quot;Elencare i flussi di attivazione di destinazione e mostrare quali sono abilitati o disabilitati.&quot; |
| **Controllare un flusso di destinazione** | &quot;Visualizza la configurazione completa per l&#39;ID flusso di destinazione `xyz789`.&quot; |
| **Verifica stato account di destinazione** | &quot;Elenca gli account di destinazione e contrassegna quelli in stato di errore.&quot; |
| **Monitorare le esecuzioni recenti dell&#39;attivazione** | &quot;Mostra flusso eseguito dalle ultime 24 ore e segnala eventuali errori.&quot; |
| **Analisi di un&#39;esecuzione non riuscita** | &quot;Visualizza la cronologia di esecuzione per l&#39;ID di flusso `xyz789` e riepiloga eventuali errori.&quot; |
| **Elenca flussi di origine** | &quot;Elencare i flussi di acquisizione di origine e visualizzarne lo stato corrente.&quot; |
| **Controllare un flusso di origine** | &quot;Visualizza la configurazione per l&#39;ID flusso di origine `src456`: cosa viene acquisito e dove arriva?&quot; |
| **Verifica integrità esecuzione acquisizione** | &quot;Mostra la cronologia delle esecuzioni recenti per l&#39;ID del flusso di origine `src456` e gli errori dei flag.&quot; |
| **Elenca gli spazi dei nomi delle identità** | &quot;Quali spazi dei nomi di identità sono configurati nella sandbox?&quot; |
| **Elenca criteri di unione** | &quot;Elenca i criteri di unione e mostra il criterio predefinito.&quot; |
| **Trovare l&#39;ID organizzazione** | &quot;Elenca le organizzazioni Adobe a cui ho accesso.&quot; |

## Accesso e abilitazione {#mcp-access}

>[!AVAILABILITY]
>
>Il server MCP di Real-Time CDP si trova in Beta e non è aperto per la registrazione self-service. L’accesso avviene solo su invito e richiede che l’organizzazione Adobe sia inserita nell&#39;elenco Consentiti in modo esplicito prima che sia possibile connettersi.

Per richiedere l&#39;accesso:

1. Contatta il rappresentante del tuo account Adobe (Customer Success Manager, Technical Account Manager o Account Executive) ed esprimi il tuo interesse per il programma Real-Time CDP MCP Beta.
2. Il rappresentante Adobe si coordinerà con il team di prodotto per valutare l’idoneità e abilitare l’ID organizzazione.
3. Una volta abilitato, il rappresentante Adobe confermerà l’accesso e fornirà ulteriore materiale di onboarding.

>[!NOTE]
>
>Solo le organizzazioni che sono state abilitate in modo esplicito possono connettersi al server MCP di Real-Time CDP. Il tentativo di connessione prima dell’abilitazione genera un errore di autenticazione.

## Prerequisiti {#mcp-prerequisites}

Prima di collegare il server Real-Time CDP MCP al client MCP, verificare quanto segue:

* Hai una licenza Real-Time CDP attiva.
* La tua organizzazione Adobe è stata abilitata per il programma Beta dal tuo rappresentante Adobe (vedi [Accesso e abilitazione](#mcp-access)).
* Si dispone dell&#39;accesso a un client MCP supportato come [!DNL Claude], [!DNL ChatGPT], [!DNL Claude Code], [!DNL Codex], [!DNL Cursor] o [!DNL VS Code].
* Hai il tuo ID organizzazione e il nome della sandbox su cui desideri eseguire la query.
* In Adobe Experience Platform disponi delle autorizzazioni necessarie per visualizzare tipi di pubblico, destinazioni ed entità del servizio di flusso.

## Collegare il server Real-Time CDP MCP {#mcp-connect}

L&#39;endpoint del server MCP di Real-Time CDP è:

```
https://rtcdp-mcp.adobe.io/mcp
```

Il server utilizza un **trasporto HTTP remoto (Streamable HTTP)** con un **flusso di accesso Adobe basato su browser**. In ogni client, il modello di configurazione è lo stesso:

1. Aggiungi l&#39;URL del server: `https://rtcdp-mcp.adobe.io/mcp`
2. Salva o abilita la connessione.
3. Completa l&#39;accesso ad Adobe basato su browser **&#x200B;**&#x200B;la prima volta che il client richiama uno strumento.
4. Fornire `imsOrgId` e `sandboxName` all&#39;inizio di ogni sessione.

### Configurazione JSON generale {#mcp-connect-json}

Per i client che accettano una configurazione del server MCP basata su JSON, ad esempio Claude Desktop (`claude_desktop_config.json`), VS Code o qualsiasi client che legge un file `mcp.json`, utilizzare uno dei seguenti formati a seconda che il client supporti HTTP remoto nativo o richieda un bridge locale:

**Tramite bridge `mcp-remote` (Claude Desktop e altri client che richiedono un bridge locale)**

```json
{
  "mcpServers": {
    "rtcdp": {
      "command": "npx",
      "args": [
        "mcp-remote",
        "https://rtcdp-mcp.adobe.io/mcp"
      ]
    }
  }
}
```

**HTTP remoto nativo (client che lo supportano direttamente)**

```json
{
  "mcpServers": {
    "rtcdp": {
      "url": "https://rtcdp-mcp.adobe.io/mcp",
      "transport": "http"
    }
  }
}
```

>[!NOTE]
>
>Nella configurazione non sono necessari chiavi API, token Bearer o intestazioni aggiuntive. L’autenticazione viene gestita interamente tramite il flusso di accesso di Adobe basato su browser al primo utilizzo.

### Eseguire l’installazione in client basati sull’interfaccia utente {#mcp-connect-ui}

#### Claude

Per `claude.ai` e Claude Desktop, aggiungere il server Real-Time CDP MCP come **connettore personalizzato** utilizzando l&#39;URL del server `https://rtcdp-mcp.adobe.io/mcp`.

* **Piani individuali** — In Claude, passare a **Personalizza connettori →**, selezionare **Aggiungi connettore** e immettere l&#39;URL del server.
* **Piani team e aziendali** — Un&#39;area di lavoro **Proprietario** o **Proprietario principale** aggiunge il connettore in **Impostazioni organizzazione → Connettori**. Una volta aggiunto, ogni utente lo abilita nelle proprie impostazioni Claude.

Dopo aver aggiunto il connettore, attivalo in una conversazione e completa l’accesso al browser Adobe al primo utilizzo. Claude individua automaticamente il server di autorizzazione di Adobe. Non è richiesto alcun ID client o segreto client.

#### ChatGPT

In [!DNL ChatGPT], aggiungi il server Real-Time CDP MCP come **connettore personalizzato**:

1. Passa a **Impostazioni → Connettori** (o **Impostazioni → App e Connettori**, a seconda del piano).
2. Selezionare **Aggiungi connettore** e immettere `https://rtcdp-mcp.adobe.io/mcp` come URL del server.
3. Salva il connettore. A seconda del piano [!DNL ChatGPT], questo passaggio potrebbe richiedere l&#39;approvazione di **Modalità sviluppatore** o dell&#39;amministratore dell&#39;area di lavoro.
4. Una volta abilitato il connettore, effettua l’autenticazione tramite il browser Adobe, accedi quando richiesto al primo utilizzo.

#### Cursore

In Cursore, aggiungi il server MCP di Real-Time CDP come server MCP remoto:

1. Apri **Impostazioni → MCP**.
2. Selezionare **Aggiungi nuovo server** e immettere `https://rtcdp-mcp.adobe.io/mcp` come URL del server.
3. Seleziona **connetti** per attivare l&#39;accesso e l&#39;autenticazione Adobe basati su browser.

Una volta connessi, gli strumenti Real-Time CDP sono disponibili nelle modalità Compositore cursore e Agente.

#### Altri client basati su interfaccia utente

Per client quali VS Code o altre applicazioni desktop e Web con supporto MCP remoto, aggiungere il server MCP Real-Time CDP come server HTTP **remoto** utilizzando `https://rtcdp-mcp.adobe.io/mcp`. Se il client supporta intestazioni o token Bearer opzionali, lasciali vuoti: al primo utilizzo l’autenticazione viene gestita tramite il flusso di accesso di Adobe basato su browser.

### Installazione in client tecnici {#mcp-connect-technical}

#### Claude Code

Aggiungere il server dal terminale:

```bash
claude mcp add --transport http rtcdp https://rtcdp-mcp.adobe.io/mcp
```

Quindi avvia Claude Code ed esegui:

```text
/mcp
```

Seleziona il server `rtcdp` e completa il flusso di accesso di Adobe nel browser. Se il server è già stato aggiunto in `claude.ai`, potrebbe essere visualizzato automaticamente in Claude Code quando entrambi sono connessi allo stesso account.

#### Codice

Aggiungere il server dal terminale:

```bash
codex mcp add rtcdp --url https://rtcdp-mcp.adobe.io/mcp
```

Autentica il server:

```bash
codex mcp login rtcdp
```

Verifica la configurazione:

```bash
codex mcp list
```

È inoltre possibile aggiungere il server direttamente a `~/.codex/config.toml`:

```toml
[mcp_servers.rtcdp]
url = "https://rtcdp-mcp.adobe.io/mcp"
```

### Parametri di richiesta richiesti {#mcp-connect-params}

Ogni chiamata allo strumento richiede due parametri che definiscono l’ambito della richiesta al tenant Adobe Experience Platform:

* `imsOrgId` — l&#39;ID organizzazione, mappato all&#39;intestazione `x-gw-ims-org-id` nelle chiamate API di Experience Platform a valle.
* `sandboxName` — nome della sandbox di Experience Platform mappato all&#39;intestazione `x-sandbox-name`.

Forniscili all’inizio di ogni sessione. Ad esempio:

> &quot;Usa organizzazione `1234ABCD@AdobeOrg` e sandbox `prod` per questa sessione.&quot;

Se non conosci il tuo ID organizzazione, chiedi all&#39;assistente AI di chiamare `search_organizations`, in modo che restituisca tutte le organizzazioni a cui le tue credenziali Adobe possono accedere.

## Limitazioni note (Beta) {#mcp-limitations}

Le seguenti limitazioni si applicano alla versione corrente di Beta del server MCP [!DNL Adobe Real-Time CDP]:

| Limitazione | Descrizione | Soluzione alternativa |
| --- | --- | --- |
| **Superficie di sola lettura** | Il server MCP espone solo le API di recupero. Non puoi creare, aggiornare, attivare o eliminare tipi di pubblico, destinazioni o flussi di dati. | Utilizza l’interfaccia utente di Real-Time CDP o le API REST di Experience Platform per le operazioni di scrittura. |
| **Nessuna metrica di coinvolgimento o consegna** | Il server MCP non restituisce le statistiche di consegna downstream, coinvolgimento o metriche di conversione dalle piattaforme di destinazione. | Utilizza la funzione di reporting della piattaforma di destinazione, Customer Journey Analytics MCP o Adobe Analytics MCP, per i dati di coinvolgimento e conversione. |
| **La query del segmento deve essere creata esternamente** | `Preview Audience Membership` richiede un&#39;espressione PQL o SDD valida come input. Il server MCP non compone la query. | Crea l’espressione PQL/SDD nell’interfaccia utente di Segment Builder o tramite l’API del servizio di segmentazione, quindi incolla nel prompt MCP. |
| **Paginazione tramite token di continuazione** | Gli strumenti elenco restituiscono risultati impaginati. L&#39;enumerazione completa in sandbox molto grandi richiede il concatenamento di `continuationToken` chiamate. | Eseguire query limitate utilizzando i filtri (nome, stato, specifica di connessione, intervallo di tempo) anziché enumerare l&#39;elenco completo. |
| **Il filtro dell&#39;esecuzione dell&#39;attivazione è basato solo sul tempo** | `Inspect Activation Runs` supporta il filtro per stato e timestamp di completamento (epoca ms UTC), ma non direttamente per tipo di errore o piattaforma di destinazione. | Filtra per `flowId` prima (ottenuto da `List Configured Destinations`) per eseguire l&#39;ambito in una destinazione specifica. |
| **ID organizzazione richiesto all&#39;inizio della sessione** | Ogni chiamata allo strumento (tranne `search_organizations`) richiede `imsOrgId` e `sandboxName` come parametri espliciti. Se non vengono fornite, le chiamate allo strumento avranno esito negativo. | All&#39;inizio di ogni sessione, comunica all&#39;assistente AI: &quot;Utilizza l&#39;organizzazione `<YOUR_ORG_ID>` e la sandbox `<SANDBOX_NAME>` per questa sessione.&quot; Se non conosci il tuo ID organizzazione, chiama prima `search_organizations`, per restituire le organizzazioni a cui le tue credenziali possono accedere. |

## Domande frequenti {#mcp-faq}

+++Quali client MCP sono supportati?

Il server MCP di Real-Time CDP funziona con qualsiasi client che supporta server MCP remoti o connettori personalizzati, inclusi [!DNL Claude], [!DNL ChatGPT], [!DNL Claude Code], [!DNL Codex], [!DNL Cursor] e [!DNL VS Code]. Il flusso di installazione dipende dal client: i client basati sull’interfaccia utente in genere aggiungono il server da un pannello di impostazioni o connettori, mentre i client tecnici come Claude Code e Codex possono aggiungerlo dalla riga di comando o dai file di configurazione.
+++

+++Come posso ottenere l’accesso?

L&#39;accesso è su invito solo durante il Beta. Contatta il rappresentante del tuo account Adobe (Customer Success Manager, Technical Account Manager o Account Executive) per richiedere l’iscrizione. Il rappresentante Adobe si coordinerà con il team di prodotto per abilitare la tua organizzazione. Per informazioni dettagliate, vedere [Accesso e abilitazione](#mcp-access).
+++

+++Come funziona l’autenticazione?

L&#39;autenticazione viene gestita tramite un accesso basato su **browser**. Quando il client MCP richiama uno strumento, apre il browser predefinito a una pagina di accesso di Adobe. Dopo aver autenticato e autorizzato il client, la sessione viene stabilita e le successive chiamate allo strumento lo riutilizzano. Non è necessario archiviare chiavi API o credenziali di lunga durata nella configurazione client.
+++

+++A quali oggetti Real-Time CDP è possibile accedere tramite MCP?

Puoi accedere a tipi di pubblico, tipi di destinazione, account di destinazione configurati, flussi di dati di destinazione, connessioni di origine e di destinazione e cronologia dell’esecuzione dell’attivazione. Le operazioni sono di sola lettura (recupero API); le operazioni di scrittura non sono supportate nella versione corrente.
+++

+++È necessario l&#39;accesso per sviluppatori per utilizzare il server Real-Time CDP MCP?

No. Il server MCP è progettato sia per utenti tecnici che di marketing. Gli addetti al marketing possono interagire con esso utilizzando prompt in linguaggio naturale in qualsiasi client MCP supportato, mentre i data engineer e gli sviluppatori possono utilizzarlo in strumenti per sviluppatori che supportano MCP.
+++

