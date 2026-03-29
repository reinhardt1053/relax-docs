---
description: Utile per applicare delle promozioni ai prodotti in scadenza
---

# Come gestire le etichette sconto

Se hai alcuni specifici pezzi di un prodotto che sono vicini alla data di scadenza potrebbe essere una buona idea metterli in promozione (es. sconto 30%) al fine di venderli velocemente prima della data di scadenza imminente.&#x20;

Relax ti consente di stampare delle etichette con un barcode che contiene codificato all'interno una percentuale di sconto che decidi tu. Durante la vendita chi sta alla cassa farà due scansioni:&#x20;

1. La prima scansione al barcode del prodotto che aggiunge il prodotto allo scontrino;
2. La seconda scansione al barcode dello sconto attaccata allo stesso prodotto, che applica lo sconto al prodotto aggiunto allo scontrino al passo precedente.&#x20;

La prima cosa da fare, per abilitare le etichette sconto in Relax, é fissare un prefisso per i barcode delle etichette sconto. Vai nella sezione **Gestione->Impostazioni->Articoli** e posizionati nella tab **Barcode** ed indica un prefisso per i barcode lle etichette sconto nel campo **Prefisso Barcode Sconto**.

![Impostazione del prefisso barcode sconto a 9999](<../.gitbook/assets/Screenshot 2021-03-03 at 05.58.43.png>)

&#x20;Un esempio di barcode sconto valido potrebbe essere: &#x20;

```
9999000000304
```

Questo barcode contiene codificata la percentuale sconto del 30%.&#x20;

{% hint style="info" %}
La lunghezza é 13 caratteri di cui l'ultimo carattere rappresenta il checksum.
{% endhint %}

A questo punto possiamo andare nella fase di cassa, aggiungere un prodotto allo scontrino e successivamente fare la scansione dell'etichetta sconto.&#x20;

![Lettura dell'etichetta sconto](<../.gitbook/assets/Screenshot 2021-03-03 at 06.14.44.png>)

Dopo la lettura dell'etichetta sconto Relax applicherá la percentuale sconto codificata nell'etichetta:&#x20;

![L'etichetta ha applicato il 30% al prodotto precedentemente aggiunto](<../.gitbook/assets/Screenshot 2021-03-03 at 06.16.40.png>)

## Invio delle etichette sconto a Passepartout

Lato Passepartout vogliamo avere un informazione che ci indica che su quella riga scontrino é stata applicata uno sconto letto tramite le etichette sconto. Vogliamo in altre parole distinguere tra uno sconto applicato da una promozione standard (**Gestione->Tabelle->Promozioni)** ed uno sconto proveniente dalla lettura di un'etichetta sconto.&#x20;

Per farlo Relax manda per ogni riga documento, nel file json di Shaker, il campo Tipo Promo. Tipo Promo é un campo di tipo intero che assumerá i seguenti valori:&#x20;

| Tipo Promo  | Significato                 |
| ----------- | --------------------------- |
| 0           | Nessuna promozione          |
| 1           | Promozione Standard         |
| 2           | Promozione Etichetta Sconto |

Per mandare questa informazione devi prima definire una videata aggiuntiva in Passepartout ed indicare l'indice della videata nella sezione di Relax **Gestione->Impostazioni->Mexal->Impostazioni Avanzate->Indice Videata Documenti Righe Tipo Promo**

![Indice videata Documenti Righe Tipo Promo impostata ad 1](<../.gitbook/assets/Screenshot 2021-03-03 at 06.26.51.png>)

Nel file json Relax manda, per ogni riga, il  campo Tipo Promo e l'indice della videata da usare:&#x20;

![I campi tipo\_promo e tipo\_promo\_videata vengono mandati a Passepartout da Relax-Shaker](<../.gitbook/assets/Screenshot 2021-03-03 at 06.56.16.png>)
