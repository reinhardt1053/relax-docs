# Gestione multiazienda

Per ogni azienda é necessario creare un database separato (sqlite o mysql). Nel caso in cui vogliamo gestire due aziende bisogna creare due config.xml (es. configAzienda1.xml e configAzienda2.xml) in C:\ProgramData\Relax. Ogni config punterá ad un database diverso.

Crea quindi due collegamenti sul desktop a relax.exe ed usa il flag --config per indicare il config.xml che ciascun exe deve usare.



**Collegamento per Azienda 1**:

relax.exe --config=configAzienda1.xml

**Collegamento per Azienda 2**:

relax.exe --config=configAzienda1.xml



Graficamente:

![](<.gitbook/assets/multiconfig (1).PNG>)

Entrando in relax con il primo collegamento si puó procedere a cambiare le impostazioni database dal menu Gestione->Impostazioni->Impostazioni Database.&#x20;

In questa configurazione si ha un solo relax.exe e piú collegamenti sul desktop che puntano allo stesso .exe ma con parametri di avvio diversi (uno per ogni azienda). Facendo l'aggiornamento verranno aggiornate entrambe i database al primo avvio delle rispettive aziende.&#x20;
