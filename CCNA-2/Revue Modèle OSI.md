
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
1. **Physique**: touts ce qui est physiques (câbles, PC, fibre optique). Les données sont appelées **bit**.

2. **Liaison de données**: liaison entre switch et switch par exemple. On peut aussi tester ici si il y  a des erreurs physiques dans le réseau (utilisation des adresses physique c-a-d **MAC**). Utilise le protocole **ARP**(traduction d'un adresse IP en adresse MAC).

3. **Réseau**: Assure la connectivité entre les hôtes dans différents réseaux. Utilise le protocole **IP** donc il assure l'**adressage IP** et l'**adressage logique**. Les données ici sont appelées **des paquets**. 

4. **Transport**: c'est ici que commence l'**encapsulation**. Elle **segmente** les données(les données dans la couche 4 sont appelées **segment**).

5. **Session**: contrôle la session entre les machines

6. **Présentation**: **encryptions** des données quand on l'envoie et **décryptions** si on le reçoit. 

7. **Application**: c'est la couche la plus haute donc la plus **proche** de l'utilisateurs finaux .

![[WhatsApp Image 2025-06-18 at 09.43.05.jpeg]]


> **P**our **L**a **R**oute **S**uis **P**apa **A**ndry


