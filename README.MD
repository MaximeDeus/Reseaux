TP3: Interrogation Serveur DNS
=====================

#### AUTEURS: DEROISSART Maxime @deroissart | SASU Daniel @sasu

> **Note:** Toute manipulation(commande) d�crite dans ce fichier est effectu�e depuis le dossier
> racine du projet.

Contenu
=======

* [Pr�sentation du TP et de ses objectifs](#pr�sentation-du-tp-et-de-ses-objectifs)
* [Arborescence Du Projet](#arborescence-du-projet)
* [Lancer le programme](#lancer-le-programme)



Pr�sentation du TP et de ses objectifs
======================================

   - Cr�er une requ�te DNS
   - L'envoyer � un serveur DNS
   - R�cup�rer la trame
   - Afficher les alias ainsi que les adresses IP de type v4 et v6


Arborescence Du Projet
----------------------
```
$ .
+-- pom.xml
+-- README.md
+-- src
    +-- main
    ��� +-- java
    ���     +-- fil
    ���         +-- rsx
    ���             +-- DNSsimple.java
    ���             +-- ReceiveUDP.java
    ���             +-- ReponsesTP3.java
    ���             +-- SendUDP.java
    +-- test
        +-- java
            +-- fil
                +-- rsx


```


Lancer le programme
------------------------------

Il y a deux fa�on possibles de lancer le programme: 

1- Lancer Eclipse
```
   Aller dans File/Import/Maven/Existing Maven Projects
   Charger le projet
   Aller dans Run/Run configurations
   Effectuer un clic droit sur Java Applications et en cr�er un nouveau
   Dans projet devrait �tre �crit tp3-interrogation-serveur-DNS_sasu_deroissart
   Dans main class �tre �crit fil.rsx.ReponsesTP3
   Aller dans Arguments
   Entrer le nom de domaine dans le cadre Program arguments:
   Cliquer sur run
```

2- Lancer le terminal
   Entrer les commandes suivantes:

```
$ mvn package
$ java -classpath target/classes fil.rsx.ReponsesTP3 (Nom de domaine du site)
$ mvn clean

```
