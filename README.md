# Blueprint-Reminders-with-actionable-Alexa-and-push-notifications


Mi è venuto in mente di avviare questo progetto perché sto constatando un certo declino nella mia memoria con l'avanzare dell'età. Per rendere più chiaro il concetto, ho preso in considerazione il caso di mio figlio, che durante i periodi influenzali o in particolari stagioni necessita di assumere diversi farmaci. Fino ad ora, avevo impostato degli allarmi sul calendario, ma questo non era sufficiente a ricordarmi tutto. Così, ho pensato di sfruttare Home Assistant e Alexa per darmi una mano.

Questo progetto è estremamente intuitivo da utilizzare. È importante notare che, per ricevere le notifiche push (anche se non obbligatorie), è necessario avere installata l'app companion. Inoltre, per interagire con Alexa, occorre utilizzare il lavoro di Keaton Taylor.

A quel punto, all'orario stabilito, e nei giorni stabiliti sui dispositivi stabiliti riceverai una richiesta da Alexa e una notifica push. Se rispondi in maniera positiva a Alexa o interagisci con la notifica push, non riceverai ulteriori promemoria. In caso contrario, trascorso il tempo impostato, riceverai una nuova richiesta da Alexa e una nuova notifica.

Puoi scaricare il progetto dal seguente il [link](https://community.home-assistant.io/t/reminders-with-actionable-alexa-and-push-notifications/723979). 

![image](https://github.com/Home-Assistant-Pro-Team/Blueprint-Reminders-with-actionable-Alexa-and-push-notifications/assets/62516592/4f72d1cc-46cb-41ed-a65b-0bc0d6f77795)


Vediamo nel dettaglio come compilare al meglio il blueprint:

- Orario notifica: Impostiamo l'orario in cui vogliamo ricevere l'avviso.
- Text notify: Scriviamo il testo dell'avviso
- Data Inizio: Impostiamo se necessaria la data inizio in cui deve iniziare a mandare il promemoria, se nel caso la data non viene modificata viene considerato da oggi.
- Data fine: Impostiamo se necessaria la data fine in cui deve smettere di mandare il promemoria, se nel caso la data non viene modificata viene inviata per sempre. Nel momento in cui la data odierna è superiore alla data impostato e solo se abbiamo impostato almeno un device mobile, riceviamo una notifica per ricordare di cancellare l'automazione con una action che vi riporterà immediatamente alla schermata dell'automazione.
- Tempo ripeti: Impostiamo un tempo in cui il singolo promemooria deve ripetersi, attenzione questo è l'unico campo obbligatorio.
- Dispositivo Alexa: possiamo selezionare il dispositivo dove ricevere il promemoria in alternativa la notifica verrà riprodotta in modo randomico.
- Dispositi mobile per notifiche: Inseriamo i dispositivi mobile che devono ricevere la notifica. 
