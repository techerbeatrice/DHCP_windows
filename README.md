# DHCP sur windows Server : installation, configuration et test

✔Configuration de la carte réseau en Réseau Interne d'une machine virtuelle qui va servir de serveur DHCP sur windows Server.

![image](https://github.com/techerbeatrice/DHCP_windows/assets/138071140/86ff4ad4-898a-4149-a9d7-aad5d082715c)

✔ Donner le rôle DHCP à windows Server, pour cela aller dans Gérer --> Ajouter des rôles et fonctionnalités --> Dans Type d'installation, sélectionner Installation basée sur un rôle ou une fonctionnalité --> Dans sélection du serveur --> Sélectionner un serveur du pool de serveurs --> Sélectionnner le serveur de destination --> Dans la liste des rôles, cochez Serveur DHCP

![image](https://github.com/techerbeatrice/DHCP_windows-server/assets/138071140/ec8351da-245a-4833-8db1-194e5bd42969)

![image](https://github.com/techerbeatrice/DHCP_windows-server/assets/138071140/f7ca0e84-ca36-486b-b004-5f5d728a6bbc)

![image](https://github.com/techerbeatrice/DHCP_windows-server/assets/138071140/5b670191-fc39-402c-9880-2bc5d9387fce)


✔Tableau de bord du gestionnaire du serveur

![image](https://github.com/techerbeatrice/DHCP_windows/assets/138071140/b329e517-c561-477b-92ba-e664e932d9e7)

✔Pour changer le nom du serveur 

![image](https://github.com/techerbeatrice/DHCP_windows/assets/138071140/25027ca0-f07e-4165-9b14-9e89ca437e10)

![image](https://github.com/techerbeatrice/DHCP_windows/assets/138071140/37dc76b1-339f-40ec-8930-d409a57690d1)

✔Pour donner une adresse IP au serveur, pour cela ouvrir Centre Réseau et Partage --> Modifier les paramètres de la carte --> Clique-droit sur Ethernet --> Propriétés --> Double-Clic sur Protocole Internet version 4 (TCP/IPv4) --> Dans Utiliser l'adresse suivante : _renseigner une adresse IP_ puis cocher _Valider les paramètres_ en quittant.

![image](https://github.com/techerbeatrice/DHCP_windows/assets/138071140/707ff9bc-eea1-43d2-9ca4-1c3cc22b07b8)

✔Configuration du serveur DHCP pour qu'il fournisse des adresses IP de la plage 172.20.0.100 à 172.20.0.200 sur le réseau 172.20.0.0/24

![image](https://github.com/techerbeatrice/DHCP_windows/assets/138071140/59144dfb-a6b2-4c4a-9d38-37b784cd8d2b)

✔Configuration de la carte réseau en Réseau Interne de la machine cliente sous windows.

![image](https://github.com/techerbeatrice/DHCP_windows/assets/138071140/60dcc39e-9fed-45b8-8e58-69c47432fd54)

✔Réservation statique de l'adresse IP 172.20.0.10 par le serveur DHCP à la machine cliente, en renseignant l'adresse MAC de celle-ci.

![image](https://github.com/techerbeatrice/DHCP_windows/assets/138071140/37eb82e3-45f9-4f47-83a8-c6077ed66179)

Le serveur DHCP a bien attribué l'adresse IP 172.20.0.10 à la machine cliente.

![image](https://github.com/techerbeatrice/DHCP_windows-server/assets/138071140/ee24476f-9ea3-44b9-b170-c5126d5b1b8e)

et même si la machine cliente perd l'adresse IP 172.20.0.10 qui lui a été attribuée par le serveur DHCP avec la commande ipconfig /release,
en refaisant une nouvelle demande d'adresse IP avec la commande ipconfig /renew, la même adresse lui est à nouveau attribuée par le serveur DHCP.

![image](https://github.com/techerbeatrice/DHCP_windows-server/assets/138071140/c122a47a-9f9a-4fd1-b6e4-f2a7ce23a5dc)



