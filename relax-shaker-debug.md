# Relax Shaker Debug

Per impostare Relax Shaker in modalitá debug, creare un file relax-shaker.properties con il seguente contenuto e salvarlo nella home dell'utente:

```
handlers=java.util.logging.ConsoleHandler, java.util.logging.FileHandler
.level=FINEST
java.util.logging.FileHandler.pattern=%h/relax-shaker.log
java.util.logging.FileHandler.limit = 50000
java.util.logging.FileHandler.count = 100
java.util.logging.FileHandler.formatter = java.util.logging.SimpleFormatter

java.util.logging.SimpleFormatter.format= %1$tF %1$tT %4$s :  %5$s%6$s%n 

```
