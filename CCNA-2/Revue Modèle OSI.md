
> [!NOTE] Encapsulation
> c'est le fait d'ajouter une **entête** à chaque fois qu'une données passe une couche dans le modèles **OSI** par exemple
> **exemple**: couche1 PDU = bit


> [!NOTE] Paquets # Trame
> 


> [!NOTE] PDU: Protocol Data Unit
> Entête définit les protocoles dans chaque couches
> Permet d'identifier un message en fonction de sa position


![[WhatsApp Image 2025-06-18 at 09.36.41.jpeg]]

> [!NOTE] Broadcast # Multicast # Unicast



Il y a **7 couches** dans le modèles **OSI** dont:
![[7couches.png]]

-  **couche 7: Application**: 
	c'est la couche la plus haute donc la plus **proche** de l'utilisateurs finaux. C’est donc elle qui va apporter à l’utilisateur les services de base offerts par le réseau, comme par exemple le transfert de fichier, la messagerie…

- **couche 6: Présentation**: 
	**encryptions** des données quand on l'envoie et **décryptions** si on le reçoit. Cette couche s’intéresse à la syntaxe et à la sémantique des données transmises : c’est elle qui traite l’information de manière à la rendre compatible entre tâches communicantes.
	Typiquement, cette couche peut convertir les données, les reformater, les crypter et les compresser.

 - **couche 5: Session**: 
	 Cette couche organise et synchronise les échanges entre tâches distantes c'est à dire contrôle la session entre les machines. Elle établit également une liaison entre deux programmes d’application devant coopérer et commande leur dialogue.

-  **couche 4: Transport**: 
	c'est ici que commence l'**encapsulation**. Cette couche est responsable du bon acheminement des messages complets au destinataire.
	Le rôle principal de la couche transport est de prendre les messages de la couche session, de les découper s’il le faut en unités plus petites et de les passer à la couche réseau, tout en s’assurant que les morceaux arrivent correctement de l’autre côté.
	Ici les données sont appelées des **segments**

- **couche 3: Réseau**: 
	C’est la couche qui permet de gérer le sous-réseau, le routage des paquets sur ce sous-réseau et l’interconnexion des différents sous-réseaux entre eux.
	Ici les données sont appelées des **paquets**.

- **couche 2: Liaison de données**: 
	Son rôle est un rôle de « **liant** » : elle va transformer la couche physique en une liaison a priori exempte d’erreurs de transmission pour la couche réseau. Elle fractionne les données d’entrée de l’émetteur en **trames**, transmet ces trames en séquence et gère les trames d’acquittement renvoyées par le récepteur.
	La couche liaison de données doit être capable de renvoyer une trame lorsqu’il y a eu un problème sur la ligne de transmission. De manière générale, un rôle important de cette couche est la **détection et la correction d’erreurs** intervenues sur la couche physique.
	Ici les données sont appelées des **trames**

- **couche 1: Physique**: 
	La couche physique s’occupe de la transmission des bits de façon brute sur un canal de communication. Cette couche doit garantir la parfaite transmission des données (un bit 1 envoyé doit bien être reçu comme bit valant 1). 
	Ici les données sont appelées des **bits**.

![[WhatsApp Image 2025-06-18 at 09.43.05.jpeg]]


> **P**our **L**a **R**oute **S**uis **P**apa **A**ndry


