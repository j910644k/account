---

copyright:
  years: 2015, 2019
lastupdated: "2019-05-29"

keywords: troubleshoot account, account problem, account support, account help, org error, resource error, error message

subcollection: account
---

{:tsSymptoms: .tsSymptoms}
{:tsCauses: .tsCauses}
{:tsResolve: .tsResolve}
{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:tip: .tip}
{:note: .note}
{:new_window: target="_blank"}
{:troubleshoot: data-hd-content-type='troubleshoot'}

# Risoluzione dei problemi relativi alla gestione degli account
{: #managingaccounts}

I problemi generali con la gestione del tuo account potrebbero includere applicazioni diverse che hanno lo stesso nome dominio o amministratori che non riescono a visualizzare tutte le organizzazioni. In molti casi, puoi risolvere questi problemi seguendo pochi semplici passi.
{:shortdesc}


## Perché non posso accedere a un'ubicazione {{site.data.keyword.Bluemix_notm}} differente?
{: #nosecondreg}
{: troubleshoot}

Non puoi creare una nuova ubicazione perché il tuo tipo di account non lo consente.

Ricevi un messaggio di errore quando provi a creare una nuova ubicazione {{site.data.keyword.Bluemix_notm}}.
{: tsSymptoms}

Ciò è probabilmente dovuto al fatto che stai utilizzando un account Lite, che supporta lo sviluppo in una sola ubicazione pubblica. Per ulteriori informazioni sulle funzioni dell'account Lite, vedi [Account Lite](/docs/account?topic=account-accounts#liteaccount).
{: tsCauses}

Per accedere a più ubicazioni, esegui l'upgrade a un account fatturabile. Vai a **Gestisci > Account** e seleziona **Impostazioni account**. Nella sezione Upgrade dell'account, seleziona l'opzione di upgrade.
{: tsResolve}


## Perché non posso creare una nuova organizzazione?
{: #nosecondorg}
{: troubleshoot}

Provi a creare più di una singola organizzazione e disponi di un account Lite.  

Ricevi un messaggio di errore quando provi a creare una nuova organizzazione.
{: tsSymptoms}

Stai probabilmente visualizzando questo errore perché stai utilizzando un account Lite, che supporta lo sviluppo solo in una singola organizzazione. Per ulteriori informazioni sulle funzioni dell'account Lite, vedi [Account Lite](/docs/account?topic=account-accounts#liteaccount).
{: tsCauses}

Per creare una nuova organizzazione, esegui l'upgrade a un account fatturabile. Vai a **Gestisci > Fatturazione e utilizzo** e seleziona **Pagamenti**.
{: tsResolve}


## Perché non posso creare una nuova istanza del piano Lite?
{: #nosecondlite}
{: troubleshoot}

Provi a creare un'istanza supplementare ma disponi di un account Lite.

Ricevi il seguente messaggio di errore quando provi a creare una nuova istanza del piano Lite:
{: tsSymptoms}

`Unable to provision new Lite instance`

Esiste un limite di una singola istanza per ogni istanza del piano Lite per garantire che tali piani restino gratuiti. Per ulteriori informazioni sulle funzioni dell'account Lite, vedi [Account Lite](/docs/account?topic=account-accounts#liteaccount).
{: tsCauses}

Puoi creare più istanze del servizio selezionando uno dei piani di servizio fatturabili, disponibili negli account fatturabili. Per eseguire l'upgrade a un account fatturabile dalla console, vai a **Gestisci > Account** e seleziona **Impostazioni account**.
{: tsResolve}

Se non vuoi eseguire l'upgrade da un account Lite e non utilizzi più l'istanza del servizio Lite esistente, puoi eliminare l'istanza del piano Lite esistente dal dashboard e quindi creare una nuova istanza.


## Come ho superato la mia franchigia di memoria di runtime?
{: #noruntimemem}
{: troubleshoot}

Hai superato la memoria consentita per il tuo account.

Non riesci a distribuire applicazioni e ottieni un errore che indica che hai superato il limite di memoria della tua organizzazione.
{: tsSymptoms}

In un account Lite, le tue applicazioni Cloud Foundry possono utilizzare fino a 256 MB di memoria di runtime istantanea. Negli account fatturabili, esiste un limite di memoria di 2 GB.
{: tsCauses}

Se stai utilizzando un account Lite, puoi ottenere più memoria eseguendo l'upgrade a un account fatturabile. Vai a **Gestisci > Account** e seleziona **Impostazioni account**. Per ulteriori informazioni sulle funzioni dell'account Lite, vedi [Account Lite](/docs/account?topic=account-accounts#liteaccount).
{: tsResolve}

Se non vuoi eseguire l'upgrade da un account Lite ma hai delle applicazioni inattive, le puoi eliminare per liberare della memoria di runtime.


## Perché il mio account è inattivo?
{: #ts_accnt_inactive}
{: troubleshoot}

Non puoi creare un'applicazione in {{site.data.keyword.Bluemix_notm}} se il tuo account è inattivo. Per risolvere questo problema, devi contattare il team di supporto.

Quando tenti di creare un'applicazione in {{site.data.keyword.Bluemix_notm}}, viene visualizzato il seguente messaggio di errore:
{: tsSymptoms}

`BXNUI0096E: L'applicazione non è stata creata. Il tuo account non è attivo perché è stato annullato o sospeso.`

Lo stato del tuo account {{site.data.keyword.Bluemix_notm}} diventa inattivo quando l'account viene annullato o sospeso.
{: tsCauses}

Per riattivare il tuo account, apri un caso dal [centro di supporto](https://cloud.ibm.com/unifiedsupport/supportcenter){: new_window} ![Icona link esterno](../icons/launch-glyph.svg "Icona link esterno"). Includi le seguenti informazioni nel tuo caso.
{: tsResolve}

  * L'ID IBM utilizzato per accedere a {{site.data.keyword.Bluemix_notm}}.
  * Il nome dell'organizzazione in cui verrà creata la tua applicazione. Queste informazioni consentono al team di supporto di determinare se ti sono stati assegnati i ruoli o l'appartenenza corretti nella tua organizzazione.


## Perché non posso aggiungere utenti ad un'organizzazione?
{: #ts_adduser}
{: troubleshoot}

Puoi invitare utenti nella tua organizzazione solo se sei il proprietario dell'account o se sei sia un gestore che un membro dell'organizzazione.

Non riesci a visualizzare il link **Invita un nuovo utente** nella sezione **Gestisci organizzazioni**.
{: tsSymptoms}

Solo i seguenti utenti {{site.data.keyword.Bluemix_notm}}
possono invitare gli utenti in un'organizzazione:
{: tsCauses}
  * Il proprietario dell'account dell'organizzazione
  * I gestori dell'organizzazione che sono anche membri, e non collaboratori,
dell'organizzazione

In {{site.data.keyword.Bluemix_notm}},
puoi essere un membro o un collaboratore di un'organizzazione.

<dl><dt>Collaboratore</dt>
<dd>Sei un collaboratore di un'organizzazione se disponi già di un account {{site.data.keyword.Bluemix_notm}} e qualcun altro ti invita nell'organizzazione.</dd>
<dt>Membro</dt>
<dd>Sei membro di un'organizzazione se non disponi di un account {{site.data.keyword.Bluemix_notm}}, ma poi qualcuno ti invita nell'organizzazione e ti registri a {{site.data.keyword.Bluemix_notm}} tramite l'invito.</dd>
</dl>

Non puoi invitare utenti nella tua organizzazione se sei un collaboratore dell'organizzazione, anche se sei stato assegnato con un ruolo di gestore organizzazione.

Tutti i gestori organizzazione, compresi i collaboratori in un'organizzazione, possono aggiungere, modificare e rimuovere gli utenti già presenti nell'organizzazione.
{: note}

Se non riesci a inviare utenti nella tua organizzazione e per farlo hai bisogno di un ruolo differente, contatta il gestore della tua organizzazione per modificare il tuo ruolo. Per identificare il gestore della tua organizzazione, completa
la seguente procedura:
{: tsResolve}

  1. Dalla barra dei menu della console, fai clic su **Gestisci > Account** e seleziona **Contatti azienda**.
  2. Vai alla tua organizzazione e visualizza le informazioni del gestore organizzazione
sulla scheda **UTENTI**.  

Se non puoi invitare utenti perché sei un collaboratore e non un membro, devi eliminare il tuo account {{site.data.keyword.Bluemix_notm}} precedente ed essere inviato a entrare a far parte dell'account come membro dell'organizzazione. Per eliminare il tuo account precedente ed entrare a far parte dell'account come membro,
completa la seguente procedura:

  1. Contatta il [Supporto {{site.data.keyword.Bluemix_notm}} ![Icona link esterno](../icons/launch-glyph.svg "Icona link esterno")](https://cloud.ibm.com/unifiedsupport/supportcenter){: new_window} per aprire un caso di supporto e richiedere l'eliminazione del tuo account. Se hai dei dati associati al tuo
account precedente che vuoi salvare e passare al nuovo account,
includi queste informazioni nell'e-mail.
  2. Una volta eliminato il tuo account, fa sì che un utente con il ruolo di gestore
organizzazione ti inviti nell'organizzazione come gestore. Utilizza quindi l'invito per registrarti in
{{site.data.keyword.Bluemix_notm}}.


## Perché non ci sono spazi associati alla mia attuale organizzazione?
{: #ts_no_space}
{: troubleshoot}

Non puoi creare un'applicazione se non ci sono spazi associati alla tua organizzazione corrente.

Quando provi a creare un'applicazione, viene visualizzato il seguente messaggio di errore:
{: tsSymptoms}

`BXNUI0097E: Prima di poter aggiungere un'applicazione, è necessario associare almeno uno spazio alla tua organizzazione e alla tua regione. Sul Dashboard, fai clic su Crea uno
spazio. Una volta creato lo spazio, prova di nuovo. `

Le applicazioni devono essere create in uno spazio nella tua organizzazione.
{: tsCauses}

Per creare uno spazio, utilizza uno dei seguenti metodi:
{: tsResolve}

  * Dalla barra dei menu della console, fai clic su **Gestisci > Account**. Espandi **Risorse account** e fai clic su **Organizzazioni Cloud Foundry**.
  Quindi, seleziona l'organizzazione in cui vuoi creare lo spazio e fai clic su **Aggiungi uno spazio**.
  * Nell'interfaccia riga di comando {{site.data.keyword.Bluemix_notm}}, immetti `ibmcloud account space-create <space_name> -o <organization_name>`.


## Perché alcune applicazioni condividono un nome dominio?
{: #ts_domain_diff}
{: troubleshoot}

Potresti notare che diverse applicazioni condividono un URL in {{site.data.keyword.Bluemix_notm}}.

Questo problema potrebbe verificarsi se assegni la stessa rotta URL per le diverse applicazioni in uno spazio.
{: tsCauses}

Ad esempio, esegui il push dell'applicazione myApp1 a {{site.data.keyword.Bluemix_notm}} e imposti il dominio su `mynewapp.us-east.cf.appdomain.cloud`. Esegui quindi il push di un'altra applicazione myApp2 nello stesso spazio e imposti una delle sue rotte URL su `mynewapp.us-east.cf.appdomain.cloud`. La rotta è ora associata a entrambe le applicazioni.

Questo funzionamento è supportato e puoi utilizzare questa procedura affinché non si verifichino tempi di inattività per l'upgrade della tua applicazione. Per ulteriori informazioni, vedi il documento relativo a [come garantire nessun tempo di inattività](/docs/overview?topic=overview-zero-downtime).
{: tsResolve}


## Perché gli amministratori non possono utilizzare la console per visualizzare tutte le organizzazioni?
{: #ts_ui_org}
{: troubleshoot}

In qualità di amministratore, non puoi visualizzare tutte le organizzazioni per gestirle quando utilizzi la console {{site.data.keyword.Bluemix_notm}}. Puoi visualizzare e gestire solo le organizzazioni alle quali appartieni.

In qualità di amministratore, non puoi visualizzare tutte le organizzazioni dalla console.
{: tsSymptoms}

Questo funzionamento è una limitazione della console.
{: tsCauses}

Puoi utilizzare comandi come `ibmcloud account orgs` e `ibmcloud account org-create` dall'interfaccia riga di comando {{site.data.keyword.Bluemix_notm}} per gestire tutte le organizzazioni. Per un elenco completo dei comandi, immetti `ibmcloud account help`.
{: tsResolve}


## Perché non posso inviare il modulo di aggiunta delle mie informazioni sulla carta di credito?
{: #ts_addcc}
{: troubleshoot}

Non puoi inoltrare le informazioni della tua carta di credito per eseguire l'upgrade del tuo account Lite a un account fatturabile.

Il pulsante **Invia** nella pagina Aggiungi carta di credito è disabilitato.
{: tsSymptoms}

Questo problema si verifica se le tue informazioni non sono state completate correttamente nella pagina Aggiungi carta di credito.
{: tsCauses}

Completa
la seguente procedura:
{: tsResolve}

  1. Nella pagina Aggiungi carta di credito, completa tutti i campi obbligatori.
  2. Seleziona **Ho letto e accetto i termini e le condizioni IBM**
e fai clic su **Invia**.

## Come posso aggiungere una carta di credito quando l'opzione non è disponibile mediante la console?
{: #ts_ccibm}
{: troubleshoot}

Vuoi immettere una carta di credito per pagare i servizi {{site.data.keyword.Bluemix_notm}}, ma l'opzione non viene visualizzata.

Quando tenti di immettere le tue informazioni sulla carta di credito, visualizzi il seguente massaggio:
{: tsSymptoms}

`Your payments are managed through IBM.com. To view your payments and maintain your billing, you can visit the IBM.com portal which contains everything for your IBMid account.`

Fai clic su **Esplora** per accedere al sito web ibm.com, ma non vedi dove immettere le tue informazioni sulla carta di credito.

Elaboriamo in modo sicuro le transazioni sulla carta di credito tramite la console {{site.data.keyword.Bluemix_notm}}. Tuttavia, in alcuni paesi, dobbiamo effettuare ulteriori passaggi per garantire l'integrità dei dati della carta di credito. Queste richieste della carta di credito vengono completate tramite il sito web ibm.com. Entrambi i metodi garantiscono che le tue informazioni sulla carta di credito siano elaborate in modo sicuro.   
{: tsCauses}

Per fornire le tue informazioni sulla carta di credito per il pagamento, completa la seguente procedura:
{: tsResolve}

  1. Vai a [ibm.com ![Icona link esterno](../icons/launch-glyph.svg "Icona link esterno")](http://www.ibm.com){: new_window} e accedi con co gli stessi ID IBM e password che utilizzi per accedere a {{site.data.keyword.Bluemix_notm}}.
  1. Fai clic sull'icona Avatar ![Icona Avatar](../icons/i-avatar-icon.svg) e seleziona **Billing**.
  1. Fai clic su **Manage payment method**.
  1. Immetti le tue informazioni sulla carta di credito e fai clic su **Register**.

Le informazioni saranno verificate e aggiunte al tuo account {{site.data.keyword.Bluemix_notm}} come il tuo metodo di pagamento per tutti gli addebiti.
