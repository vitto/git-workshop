# Workshop GIT

![WingsItaly](https://image.ibb.co/hHRHPn/wingsitaly.jpg)

Lavoriamo per WingsItaly, la famosa compagnia aerea di bandiera e questo repository
contiene tutti i modelli che compongono la nostra flotta.

Crea un fork su un tuo repository di questo progetto per iniziare a lavorare.

## Esercitazioni

1. Il reparto acquisti comunica che sono in contrattazione per l'acquisto di un nuovo aereo.
Ci viene chiesto di predisporre il nuovo modello ma di non renderlo disponibile finché
l'acquisto non sarà effettivo. Riceviamo una mail con le caratteristiche:

```
---
name: Embraer 175
type: Regional Aircraft
seats: 88
length: 31.7
height: 9.73
wingspan: 26
cruisingSpeed: 850
seats:
  - economyClass: 80
  - economyClassConfort: 8
```

Creare il modello in un feature-branch e pushare il branch sul repository remoto.

2. Il reparto tecnico ci avvisa che le modifiche effettuate al modello **Embraer 190**
per l'aumento di posti hanno causato un sacco di problemi ai viaggiatori e che quindi
è necessario ripristinare il numero di posti originari.

Scorrere la history per trovare la modifica all'aereo e tornare alla situazione precedente.
Utilizza il comando `git revert` per risolvere l'esercizio.

3. Il reparto legal ci fa notare che nel nostro repository non c'è alcun riferimento
al modello di giubbotti di salvataggio contenuti all'interno degli aerei; informazione
fondamentale affinché il Garante dei Giubbotti di Salvataggio non ci infligga una sanzione molto salata.
Fortunatamente il modello di giubbotto è lo stesso per tutti gli aerei:

```
lifeJacket: H7-25
```

Aggiungere l'informazione a tutti i modelli disponibili.

4. Il reparto acquisti ci conferma che è stato trovato l'accordo per il nuovo modello.
Possiamo quindi aggiungerlo ufficialmente al nostro repository. Ci comunica, inoltre,
che per questo nuovo modello i giubbotti di salvataggio a disposizione saranno
di un modello differente: `Guiler`.

Mergiare il feature-branch creato al punto **1** su `master` assicurandoci prima che
esso sia allineato con tutte le modifiche effettuate sul branch principale.

------

5. Tempo fa il team di R&D iniziò un esperimento per aumentare le prestazioni dell'**Embraer 190**
e, per l'occasione, fu creato il feature branch `embraer190-improvements`. Il team ci
informa che l'esperimento è andato a buon fine e che possiamo aggiornare il nostro repository.

Portare il feature branch `embraer190-improvements` sul branch principale risolvendo
eventuali conflitti. Prima di spostare il lavoro sul branch principale modificare la history
del branch `embraer190-improvements` affinché le commit che aggiornano la velocità di crociera 
vengano accorpate in un'unica commit.
