# DHCP sur windows : installation, configuration et test

✔Configuration de la carte réseau en Réseau Interne d'une machine virtuelle qui va servir de serveur DHCP sous windows.

![image](https://github.com/techerbeatrice/DHCP_windows/assets/138071140/86ff4ad4-898a-4149-a9d7-aad5d082715c)

✔Tableau de bord du gestionnaire du serveur

![image](https://github.com/techerbeatrice/DHCP_windows/assets/138071140/b329e517-c561-477b-92ba-e664e932d9e7)

✔Pour changer le nom du serveur 

![image](https://github.com/techerbeatrice/DHCP_windows/assets/138071140/25027ca0-f07e-4165-9b14-9e89ca437e10)

![image](https://github.com/techerbeatrice/DHCP_windows/assets/138071140/37dc76b1-339f-40ec-8930-d409a57690d1)

✔Pour donner une adresse IP au serveur, ouvrir Centre Réseau et Partage --> Modifier les paramètres de la carte --> Clique-droit sur Ethernet --> Propriétés --> Double-Clic sur Protocole Internet version 4 (TCP/IPv4) --> Dans Utiliser l'adresse suivante : _renseigner une adresse IP_ puis _cocher les paramètres en quittant_.

![image](https://github.com/techerbeatrice/DHCP_windows/assets/138071140/b0acb679-f26b-43e1-a838-d472177871cb)

✔Configuration du serveur DHCP pour qu'il fournisse des adresses IP de la plage 172.20.0.100 à 172.20.0.200 sur le réseau 172.20.0.0/24

![image](https://github.com/techerbeatrice/DHCP_windows/assets/138071140/59144dfb-a6b2-4c4a-9d38-37b784cd8d2b)

✔Réservation statique de l'adresse IP 172.20.0.10 par le serveur DHCP à une machine cliente, en renseignant l'adresse MAC de celle-ci.

![image](https://github.com/techerbeatrice/DHCP_windows/assets/138071140/37eb82e3-45f9-4f47-83a8-c6077ed66179)

✔Configuration de la carte réseau en Réseau Interne de la machine cliente sous windows.

![image](https://github.com/techerbeatrice/DHCP_windows/assets/138071140/60dcc39e-9fed-45b8-8e58-69c47432fd54)





