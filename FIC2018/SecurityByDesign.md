# Security By Design

RGDP à prendre en considération dès le départ d'un projet
Normes de sécurisétion des objets connectés -> sinon difficultés à corriger par la suite

Présents:
VMWARE
Armée de Terre
Entrepreneur avec un passif de 3 entreprises en sécurité
Un speaker dans le domaine
Un Directeur d'Usine à GAZ

##Meltdown et spectre
-> Remettre en question la pile de confiance
OS sans correctifs pendant longtemps .... 

Dans le cas de Meltdown:
- difficultés à protéger
- attaque *LOGIQUE* sur le matériel
- le niveau d'attaque peut - être beaucoup plus fort

Le modèle économique des hackers n'est que de quelques millions d'euros pour mener une attaque impactante au niveau national ou plus large encore

Les points d'accès wifi, les routeurs sont des cibles (référence Miraille ?)

Question : La culture de l'insécurité n'est elle pas une bonne culture

### Un projet commence par une analyse de risque
 Périmètre 
 Ministère des armées : audit des systèmes d'armes jusqu'à l'application de commande des treillis.

- Dès le cahier des charges, la sécurité est à prendre en compte
Armée de Terre a une Fiche d'Engagement Rationnelle des Objectifs de Sécurité -> FEROS
avec les mesures de défendabilité/ de défense
Listing des menaces et des mesures

- Avoir une mal vision : plus maîtrisable par la conception, les attaques logiques sont plus maîtrisables

- VMWARE précise de se baser sur les socles de confiance. 
La première ligne pour la sécurité est le serveur qui héberge les autres serveurs
Gérer la sécurité des applications en VM (problème d'architecture)

- Au cours du cycle de vie du projet
 - Gestion des patchs et mise en place (Maintenance)
 - Si apparition du risque -> analyse de risque
 - Stratégie de détection -> prévoir de s'adapter

DONC UNE CLE EST UN SYSTEME DYNAMIQUE

La sécurité dynamique , l'adaptation des anti-virus , les parades à mettre en place doivent être adaptables.

En usine, la conception se fait avec les exploitants. 

### Les modèles 

- Modèle du château fort est résolu

- Modèle Aéroport :
 - Micro segmentation avec contrôle à chaque étape soit modèle 0 TRUST
 Autoriser uniquement le trafic légitime
 VMWARE (Add Defense) CSID
 - Se baser sur ce qui est bon, ce qui a été rédigé comme bon. Tout le reste est rejeté.

- Modèle de la Citadelle
 - positionner les bons capteurs aux bons endroits et cloisonner. Ce qui permet d'observer.
 - soit le modèle du sous-marin : si une partie est inondée, le reste tourne. Chaque ilôt à son autonomie.

Au final, Mix du tout

### La défendabilité

Défendre - surveiller (détecter) - mécanisme de remédiation
- Outils
- processus
- hommes

- Alerter
- Détecter
- Agir

SYSTEME PENSER POUR INTERVENIR

### Architecture 0 TRUST

Exemple Google Corp
- Chiffrer chaque flux
- Autoriser chaque utilisateur
- Autoriser chaque serveur

Est-ce trop ? 
C'est adapté par google est plus simple à sécuriser

Armée : l'important est de réagier et de s'adapter
Architecture oui mais surtout réactivité du système

ARAMCO
http://www.zdnet.fr/actualites/le-groupe-petrolier-aramco-cible-d-une-cyberattaque-l-acte-d-activistes-39775459.htm
http://www.lepoint.fr/high-tech-internet/l-arabie-saoudite-sous-le-feu-de-hackers-25-01-2017-2099955_47.php


### Statistiques

C'est souvent l'utilisateur par des maladresse qui permet une attaque
20 % des vulnérabilités sont exploitées par des attaques
80 % des maladresses

-> Gestion des privilèges et des contrôles d'accès
### Problématiques
SANTE

Comment intégrer les utilisateurs dans la conception?
Etude du comportement applicatif qui doit toujours êtres plus ou moins identique
Reconnaître les comportements anormaux