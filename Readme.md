# Configuration d'une adresse IP statique avec le script IP Fixe

Ce guide vous montre comment configurer une adresse IP statique sur une machine Debian en utilisant un script qui prend l'adresse IP actuellement attribuée à la machine et la configure comme adresse IP statique.

### Tout en un :
```
wget https://raw.githubusercontent.com/IsT3RiK/ip_fixe_debian/main/scriptipfixe -O set_static_ip.sh
chmod +x set_static_ip.sh
sudo ./set_static_ip.sh
cat /etc/network/interfaces
```





### Étapes :
Téléchargez le script:
Exécutez la commande suivante pour télécharger le script depuis le dépôt GitHub :


```wget https://raw.githubusercontent.com/IsT3RiK/ip_fixe_debian/main/scriptipfixe -O set_static_ip.sh```

Rendez le script exécutable:
Après avoir téléchargé le script, exécutez la commande suivante pour le rendre exécutable :



```chmod +x set_static_ip.sh```

Exécutez le script:
Cette étape définira l'adresse IP actuelle comme adresse IP statique. Assurez-vous d'avoir sauvegardé toutes les données importantes et votre configuration réseau actuelle avant de continuer :


```sudo ./set_static_ip.sh```

Vérifiez la configuration:
Après avoir exécuté le script, vous pouvez vérifier la configuration réseau actuelle avec la commande suivante :


```ip a```

Cela affiche la liste des interfaces réseau et leurs adresses IP. L'adresse IP de votre interface principale est maintenant configurée en tant qu'adresse IP statique.
