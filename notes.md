# StormShield

## I - Firewalls

### Petite Entreprise

- SN160(w)

- SN210(w)

- SN310

### Moyenne Entreprise

- SN510

- SN-M-SERIES-720

- SN-M-SERIES-920

### Grand-comptes

- SN1100

- SN2100

- SN3100

- SN6100

### Industrie

- SNi20 & SNi40

Utilisation des protocols industriels (Profinet, Modbus..).

Rupture Tolerant (Rigide, electricity independent).

- SNxr1200

Résistance à condition extemes (température -40 -> 55 , haute pression)

Respet standard militaire.

### Appliances Virtuelle

- Elastic Virtual Appliance

s'intégre dans l'hypervideur.

peut etre hebergé aussi dans les services cloud (microsoft Azure, AWS)

> les versions avec LTSB means supported for the long term.

## Administration centralisé

- Stormshield Management Center (SMC) 

Permet l'administration d'un parc complet de Firewalls StormShield.

Permet le deploiement des scripts, vpn sec, objets globaux, filtrage, surveillance des firewalls (licenses, ressources..).

## Fonctions standard

- IPS : Intrusion prevention system

- Signature contextuelles IPS : Une base de signatures d'attaque utilisé avec IPS pour renforcer les sécurité

- Antispam

- Antivirus standard

- Filtrage URL

- Systeme : 
    * raid 1
    * Double partion systeme (principale et secours)
    * Haute disponibilité

> stockage est natif dans l'ensemble des produits excepté pour les `SN160(w), SN210(w) et SN310`.

## Pack Sécurité

les différents packs sont : 

- Remote Office Security Pack: Protection des petis sites distants, connecté par un tunnel VPN.

- UTM Security Pack : bénifice IPS unique de stormsheil Network Security + antispam ...

- Premium UTM Security Pack : entreprises exigeantes en matière de securité.

- Entreprise Security Pack: concentre sur les fonctionnalités Next-Genneration Firewall.


Après le choix d'un pack, on peut ajouter les services suivants:

- Stormshield Network Vulnerability Manager

- Antivirus Avancé

- Filtrage Web Extended Web Control

- Stockage des log sur la carte SD

- Breach Fighter : Permet d'effectuer dans le Cloud une analyse complémentaire à celle de l'antivirus avanc", pour bloquer des attaques élaborées, avec le soutien d'une équipe de sécurité dédiée

## Prise en main du firewall

il existe deux comptes sur `https://mystormshield.eu/` : 

- Compte client : permet d'enregistrer l'ensemble des produits Stormshield d'une meme entreprise.

- Compte partenaire: permet des gérer l'infogérence éventuelle de comptes clients.

> L'infogérance1 est la prise en charge contractuelle, par un prestataire extérieur, d'une partie ou de la totalité des ressources informatiques d'une entreprise.

sur le site on peut:

- télécharger les licences.
- Récupérer des fichiers de conf.
...

pour le documentation : ` https://documentation.stormshield.eu`.

pour la knowledge base : ` https://kb.stormshield.eu`.

## Les composants du firewall StormShield

![alt text](image.png)

- Button démarage/arret

- Trois LED :
    * orange : firewall sous tension
    * verte : systeme d'exploitation du firewall est fonctionnel
    * verte : firewall a fini de démarrer et qu'il est fonctionnel.
- Post clavier PS2 + VGA/HDMI

> carte mémoire doit etre au minimum de class 10.

Le démarage/arret du firewall se fais en cliquant sur le button de démarage/arret.

Maintenir sur le button Rest pour 10s pour le reset.

## Configurer le firewall

![configuration du firewall](image-1.png)

> A partir de l'interface (0,0) aka top left, la premiere interface s'appelle OUT, le deuxieme IN, la troisieme DMZ1 -> DMZn

L'interface OUT est une inteface externe utilisé pour se connecté à l'internet.

les autres sont internes et servent principalement à connecter le firewall à des réseau locaux.

### le bridging:

Routing allows multiple networks to communicate independently and yet remain separate, whereas bridging connects two separate networks as if they were a single network.

![](image-2.png)

> le bridge à une adresse IP 10.0.0.254/8 + il contient un serveur DHCP, il distribue des adresse comprisent entre 10.0.0.10 - 10.0.0.100

la connection vers l'interface graphique d'administrqtion est `https://10.0.0.254/admin`

par default : 
    - login : **admin**
    - password : **admin**

## L'interface d'administration

![Interface ](image-3.png)

## Confirguration Système

Accessible par : CONFIGURATION -> SYSTEME -> Configuration.

### Configuration générale

- Les paramètres cryptographiques regroupent deux options qui sont
respectivement en relation avec les certificats (présentés dans la formation
Expert) et le mode « ANSSI Diffusion Restreinte (DR) ».

La politique de mots de passe définit la longueur minimale et les caractères
obligatoires des mots de passe créés dans les différents menus du firewall (par
exemple : mots de passe des utilisateurs dans l’aŶŶuaiƌe interne (LDAP), mots de
passe qui protègent les fichiers de sauvegarde, mots de passe des certificats créés
au niveau du firewall).

### Administration du firewall

on peut modifier la certificat SSl de l'interface de configuration.

on peut modifier le port par défaut (443/TCP).
*






 







