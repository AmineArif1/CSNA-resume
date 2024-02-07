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




