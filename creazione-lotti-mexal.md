# Creazione Lotti Mexal

Esempio di formato json riga documento per la creazione lotti:

<pre><code>{
      "tipo" : "R",
      "articolo" : "172",
      "alias" : "",
      "alias_videata" : "1",
      "alias_note" : "",
      "alias_note_videata" : "2",
      "descrizione" : "Antipasto di mare",
      "confezioni" : "0",
      "quantita" : "1.00",
      "aliquota" : "10",
      "prezzo" : "8.000000",
      "um" : "1",
      "sconto" : "10.0000",
      "provvigione" : "0.0000",
      "trasporto_codice_causale" : "0", 
      "lotti" : [
        { 
           <a data-footnote-ref href="#user-content-fn-1">"codice" : "abcd"</a>,
           "stato" : "C",
           "tipo"  : "aa",
           "scadenza" : "20250601",
           "quantita" : "4.00",
           "dati_personalizzati" : [
              {
                "codice" : "f",
                "tipo" : "A",
                "valore" : "abcd"
              },
              {
                "codice" : "s",
                "tipo" : "D",
                "valore" : "20250601"
              }
	   ]
        }
      ]
}
</code></pre>

Il meccanismo di creazione lotti si attiva se viene fornito il campo codice lotto&#x20;

[^1]: **La presenza di questo campo fa scattare la creazione del lotto mexal**
