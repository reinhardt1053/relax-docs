# Come risolvere errore "MySQL server has gone away"

### Increase wait\_timeout and max\_allowed\_packet

Lanciare la query per ottenere il valore corrente:&#x20;

```
SELECT @@wait_timeout, @@max_allowed_packet;
```

Aprire il file my.cnf e modificare i parametri:&#x20;

```
wait_timeout=28800;
max_allowed_packet=107374182
```

Riavviare il server di mysql e controllare  con la query sopra se il valore é stato modificato.&#x20;



#### Sources

[https://tableplus.com/blog/2018/11/mysql-server-has-gone-away-solved.html](https://tableplus.com/blog/2018/11/mysql-server-has-gone-away-solved.html)

###

