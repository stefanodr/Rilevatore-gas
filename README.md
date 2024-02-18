# Rilevatore Consumo GAS/ACQUA manuale:
Con questo package può essere creato un sensor template per l'inserimento del consumo del gas e dell'acqua rilevabile dalla plancia energia, con abbinati degli utility meter per i conteggi, per chi come me ha l'esigenza di monitorare i dati di consumo, ma non può o non vuole istallare rilevatori vicino ai contatori. 
Si compone di:
1. Package: "consumo_gas_1_0.yaml", "consumo_acqua_1_0.yaml" (deve essere abilitata la cartella package se non già fatto);
2. Card: "card_consumo_gas_1_0.txt", "card_consumo_acqua_1_0.txt" da inserire in plancia per rilevamento manuale del dato;
3. Immagine: "rse.png", "contatoreH2o.png" per abbellire la card, ma ovviamente può essere usata qualsiasi immagine a piacimento;
4. Visto che nei sensor template non è possibile prevedere lo state_class:
4a. Script: "add_state_class.py" (abilitare la cartella "python_scripts" in //config se non già fatto);
4b. Automazione: "Automazione.yaml" per inserire tramite lo script con un ritardo di 30 sec. lo stato "state_class: total_increasing" per il rilevamento della plancia.
Di seguito un esempio della CARD di rilevazione allegata con degli spunti con card immagine,grafico e consumi giornalieri, mensili, annuali:

![image](https://github.com/stefanodr/Rilevator99e-gas/assets/117826567/51d27855-8486-4476-957c-7f4099c1e72a)

