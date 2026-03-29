---
description: >-
  Descrive come importare le anagrafiche articoli da un file esterno
  (provenienti per esempio da un altro programma)
---

# Import Articoli

Per importare articoli da un file CSV andare nella sezione **Gestione->Servizi->Import Articoli**.

![](<.gitbook/assets/Screenshot 2020-08-10 at 11.49.57.png>)

In questa fase viene proposta una griglia in cui:&#x20;

* Nella prima colonna **Campo** sono presenti tutti i campi che Relax é in grado di acquisire
* Nella seconda colonna **Posizione** deve essere indicata la posizione di ciascun campo all'interno del file CSV (L'elemento in prima posizione ha indice 0) .&#x20;
* Il valore indicato nella terza colonna **Valore Predefinito** viene utilizzato da Relax nel caso in cui per il campo considerato é stato indicato nella colonna Posizione il valore -1.&#x20;

Puoi quindi indicare nella colonna Posizione il valore -1 per tutti quei campi che non sono disponibili nel tuo tracciato CSV, Relax userá il valore che fisserai nella colonna Valore Predefinito. &#x20;

{% hint style="warning" %}
Attenzione: la prima riga del file CSV viene ignorata, Relax si aspetta di trovare l'intestazione delle colonne CSV. I dati veri e propri si devono trovare dalla seconda riga in poi.&#x20;
{% endhint %}

Premi infine il tasto "Seleziona File" per scegliere il file CSV da importare ed attendi che la procedura termini.&#x20;
