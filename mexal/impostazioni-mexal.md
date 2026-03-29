# Impostazioni Mexal

## **Utilizza anno precedente**

Se attivo Relax sincronizza giacenze, lotti e prezzi usando indice massimo per il campo anno meno uno. Mexal usa un indice per l'anno che va da 0 a 9.&#x20;

## **Controlla Esito Invio Shaker**

In fase di conferma dello scontrino Relax controlla che il file JSON generato sia stato processato correttamente da Relax-Shaker. Relax attende 5 secondi passati i quali, se il file JSON é ancora presente nella cartella shaker, genera un avviso al cliente. Da notare che il documento é già emesso ed eventualmente anche stampato dal registratore fiscale anche nel caso in cui l'invio a Mexal fallisce.&#x20;

## Disabilita Mexal Sync in presenza di errori shaker

Questo flag blocca l'esecuzione della sincronizzazione da Mexal a Relax se ci sono dei problemi con shaker. Viene controllato che ci siano file da inviare con estensione .txt o eventuali file in errore con suffisso \_error. In tal caso il sync viene impedito e viene visualizzato un messaggio di avviso. &#x20;

## Lettura diretta credito carta prepagata

Se attivo quando si effettua la lettura della fidelity card Relax si connette direttamente al database di Mexal DB e riporta il credito disponibile nel pannello cassa. Vengono inoltre controllato lo stato di shaker e viene visualizzato un messaggio di errore nel caso in cui ci siano file da inviare o in errore.&#x20;

## Importa Barcode

Questo campo può assumere i valori S, N o vuoto. Lasciarlo vuoto equivale a S per gli articoli standard. Per gli articoli padri nel caso di taglie e colori se viene lasciato vuoto verrà usato come valore di default quanto specificato nel parametro **Importa Barcode Articoli Padre.**&#x20;

## **Importa Barcode Articoli Padre**

Se impostato a False il codice a barre dell'articolo padre nel caso di taglie e colori non verrà importato.&#x20;

## Aliquota IVA Alternativa

Se il campo aliquota IVA alternativa é valorizzato verrà preferito al campo aliquota standard di Mexal.&#x20;
