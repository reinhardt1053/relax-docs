---
description: >-
  In questo capitolo trovi le informazioni su come emettere e riscattare
  vouchers promozionali in Relax.
---

# Vouchers

Un voucher promozionale è un tipo di buono o codice che può essere utilizzato per ottenere uno sconto o altri vantaggi durante un acquisto.&#x20;

Ogni voucher é identificato da un codice univoco.  Questo codice é rappresentato come barcode o qr-code e puó essere stampato e/o inviato digitalmente attraverso i canali di marketing dell'azienda (per esempio via email, sms, whatsapp, instagram, ecc. )&#x20;

Nella forma piú semplice un voucher ha associato un importo in euro, il cliente che ha ricevuto il voucher puó recarsi presso uno dei punti vendita della tua azienda e riscattare il voucher usandolo come forma di pagamento alternativa al contante. Il voucher non é nominativo e puó essere regalato ad un'altra persona.&#x20;

Un voucher puó essere generato a partire dai punti fidelity oppure essere venduto come un normale articolo ad un prezzo stabilito, in quest'ultimo caso parliamo di Gift card.&#x20;

{% hint style="warning" %}
Per usare i vouchers é necessario effettuare il login a Relax Cloud dalla fase&#x20;

**Gestione->Impostazioni->Cloud**
{% endhint %}

Nelle prossime sezioni vedremo:

* Come creare un voucher in cambio di un numero di punti fedeltá stabilito
* Come riscattare un voucher usandolo come metodo di pagamento
* Come creare un voucher in cambio di denaro (Gift Card)

## Come creare un voucher in cambio di punti fedeltá

Per prima cosa dobbiamo definire il valore del voucher in euro, andiamo nella fase

&#x20;Gestione->Tabelle->Buoni Spesa

<figure><img src=".gitbook/assets/Capture d’écran 2024-04-01 à 17.58.36.png" alt=""><figcaption><p>Backend Gestionale Relax</p></figcaption></figure>

Clicchiamo sul tasto **Nuovo** per creare un nuovo buono spesa, indichiamo il valore (es. 5,00 euro) nel campo Prezzo di Vendita IVA Inclusa ed indichiamo Aliquota IVA = E10.&#x20;

<figure><img src=".gitbook/assets/Capture d’écran 2024-04-01 à 18.02.24.png" alt=""><figcaption><p>Gestione Buoni spesa Relax</p></figcaption></figure>

Andiamo nella scheda "Fidelity" e definiamo quanti punti sono necessari per ottenere un voucher nel campo **Punti Premio** (es 500 punti)&#x20;

<figure><img src=".gitbook/assets/Capture d’écran 2024-04-01 à 18.03.14.png" alt=""><figcaption><p>Per ottenere un voucher di 5 euro al cliente verranno scalati 500 punti dalla sua carta fidelity</p></figcaption></figure>

Clicchiamo sul tasto salva per completare questa prima fase. Abbiamo definito il taglio dei voucher che andremo ad emettere.

{% hint style="info" %}
Possiamo ripetere il processo visto per creare altri tagli possibili. Per esempio ripetiamo i passaggi e creiamo un altro buono spesa del valore di 1 euro che richiede 100 punti fidelity.&#x20;
{% endhint %}

Passiamo ora all fase di generazione dei voucher vera e propria a partire dai tagli definiti.&#x20;

Andiamo nella fase Cassa e selezioniamo un cliente con fidelity che abbia almeno 500 punti sulla sua tessera.  A questo punto clicchiamo sul tasto Chiave e poi su Fidelity Card.&#x20;

{% hint style="info" %}
Puoi inserire il tasto Fidelity Card nella sidebar di Relax dal menu Gestione->Impostazioni->Aspetto->Sidebar
{% endhint %}

<figure><img src=".gitbook/assets/Capture d’écran 2024-04-01 à 18.14.54.png" alt=""><figcaption><p>Generazioni vouchers a partire dai punti fedeltá</p></figcaption></figure>

Relax visualizza nella parte bassa di questa schermata i possibili buoni spesa che si possono generare, riportando il corrispettivo valore in punti e in euro per ciascuno di essi. Clicchiamo sul buono da 5 euro per aggiungerlo a scontrino e chiudiamo la schermata. L'articolo buono spesa é  aggiunto allo scontrino con sconto 100%, il cliente pagherá appunto con 500 punti della sua fidelity card per ottenere il voucher che verrá generato.&#x20;

<figure><img src=".gitbook/assets/Capture d’écran 2024-04-01 à 18.17.00.png" alt="" width="375"><figcaption><p>Articolo buono spesa con sconto 100%</p></figcaption></figure>

Confermiamo lo scontrino, il misuratore fiscale stamperá subito dopo lo scontrino il voucher di 5 euro con il relativo barcode.&#x20;

{% hint style="danger" %}
Per emettere un voucher é necessario che il tuo computer sia connesso ad internet.
{% endhint %}

Nella prossima sezione vedremo come riscattare il voucher emesso.&#x20;

## Come riscattare un voucher&#x20;

Il voucher che abbiamo emesso e stampato nella sezione precedente puó essere usato dal cliente  come metodo di pagamento durante un acquisto successivo, recandosi presso uno dei nostri punti vendita.&#x20;

Per prima cosa é necessario attivare il pagamento con voucher dalla fase&#x20;

Gestione->Impostazioni->Pagamenti.

<figure><img src=".gitbook/assets/Capture d’écran 2024-04-01 à 19.07.04.png" alt="" width="375"><figcaption><p>Impostazioni Pagamento con Voucher</p></figcaption></figure>

Andiamo ora in Impostazioni->ECR->Pagamenti ed assicuriamoci che sia stato attivato il pagamento con "Buoni Spesa".&#x20;

Creiamo ora un nuovo scontrino dalla fase cassa e passiamo alla fase pagamenti. Selezioniamo il metodo di pagamento "Buoni spesa". &#x20;

Possiamo effettuare la scansione del barcode presente sul voucher o digitare manualmente il voucher e premere il tasto Aggiungi.&#x20;

<figure><img src=".gitbook/assets/Capture d’écran 2024-04-01 à 18.54.32.png" alt=""><figcaption><p>Pagamento utilizzando il voucher</p></figcaption></figure>

In questo specifico esempio chiuderemo la vendita pagando il rimanente importo di 1 euro in contanti. Confermando la stampa il voucher verrá riscattato e non potrá piú essere usato in nessuno dei tuoi punti vendita. &#x20;

{% hint style="danger" %}
Per emettere e riscattare i voucher é necessario che la connessione ad internet sia attiva. Questo é necessario perché Relax Desktop usa Relax Cloud per la gestione dei voucher al fine di prevenire abusi (es. riscatto multiplo dello stesso voucher in punti di vendita differenti)
{% endhint %}

## Come  creare una Gift Card

Per creare una gift card andiamo nel menu **Gestione->Impostazioni->Buoni Spesa** e clicchiamo su Nuovo.

Digitiamo il nome della Gift card nel campo descrizione e l'importo nel campo Prezzo Vendita Iva Inclusa. &#x20;

Possiamo assegnare la nuova gift card ad una categoria articoli per facilitare la ricerca in fase di vendita.&#x20;

<figure><img src=".gitbook/assets/Capture d’écran 2024-04-01 à 19.11.12.png" alt=""><figcaption><p>Creazione di una gift card </p></figcaption></figure>

Possiamo ora andare nella fase Cassa e vendere la gift card appena creata come un qualunque altro articolo. Subito dopo la stampa dello scontrino Relax genererá e stamperá un voucher con relativo barcode per ogni gift card presente in scontrino.



&#x20;





&#x20;









