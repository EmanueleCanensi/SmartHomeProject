# SmartHomeProject
Smart Home example using Arduino yun, server on cherrypy and mqtt/rest comunication
## Come funziona?
Il progetto unisce diverse tecnologie rivolte allo sviluppo dell'Internet of Things, unisce una scheda Arduino YUN rev2 ad un server programmato in python tramite
il framework Cherrypy. Il server accetta comunicazioni tramite due diversi protocolli, sia il protocollo REST sia MQTT, quest'ultimo rivolto soprattutto alla comunicazione 
verso la scheda per alleggerirla il più possibile, inoltre permette l'inserimento di nuovi utenti, endpoint e servizi come un bot di telegram user-frienldy e una dashboard per 
tenere tutto sotto controllo. Il controllore utilizza un sensore di temperatura, un sensore di presenza e uno di rilevazione acustica e attuatori fra cui un motore FAN che simula 
un ventilatore, un led che indica il riscaldamento e una luce. In base alla presenza o meno di persone è possibile settare differenti range di temperatura nei quali far partire i
due diversi sistemi. Come modalità di comunicazione e salvataggio dei dati si è deciso di utilizzare il formato JSON.
## Altre informazioni
All'interno dei repositories denominati Laboratorio \# si possono trovare script e sketch di esempio per provare i singoli moduli con cui è stato infine creato il progetto finale.
## TODO List
Implementare il progetto esistente con metodi ancora più sicuri, leggeri e/o performanti, ad esempio riprogrammare il server su Django e realizzare il controllore con una scheda 
Arduino UNO e la presenza di un modulo ESP8266
