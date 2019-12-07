# esercizio-Inc1000 parte 1
In questo esercizio ho creato 2 oggetti con la stessa classe a cui ho assegnato un Thread,questi 2 oggetti hanno il compito di incrementare un contatore di 1000 ciascuno.
Quando si va a fare l' output si può chiamare il metodo dell' oggetto soltanto richiamando la classe,questo perchè il contatore all' interno della classe viene dichiarata statica,quindi tutti gli oggetti di quella la condividono,infatti se la variabile contatore venisse dichiarato public ci sarebbe un errore.
In output viene restituito il valore 0,questo perchè i Thread vengono fermati priva che facciano il loro incremento.

# esercizio-Inc1000 parte 2
In questo esercizio a differenza del precedente si aggiungono le chiamate ".join" ai 2 oggetti,questo per far si che i 2 thread terminino la loro esecuzione,però in alcuni casi il risultato in output non è quello desiderato,questo perche i 2 thread non sono sincronizzati,quindi alcune volte possono accedere alla stessa variabile in contemporanea senza incrementare come dovuto il contatore.

# esercizio-Inc1000 parte 3
In questo esercizio a differenza del precedente si aggiunge synchrosized al metodo run,con questa aggiunta i 2 thread si sincronizzano tra di loro e non si vengono a creare collisioni sulla variabile contatore così che ilvalore finale sarà sempre 2000.
