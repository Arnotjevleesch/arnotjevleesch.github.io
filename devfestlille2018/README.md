# DEVFEST LILLE 2018

Toutes les vidéos : https://www.youtube.com/playlist?list=PLuZ_sYdawLiUAmzsywNDAh_TPuBVylwjt

## **Bas du front**

## Keynote : Et si Mario était UX Designer

<a href="http://www.youtube.com/watch?feature=player_embedded&v=vaXPyWfangg
" target="_blank"><img src="http://img.youtube.com/vi/vaXPyWfangg/0.jpg" 
alt="Keynote : Et si Mario était UX Designer" width="240" height="180" border="2" align="right"/></a>

*Alexandra Nemery & Sarah Colmon - Murex*

Un constat : le sujet est moins valorisé en France qu'aux US

4 personnalités : explorateur, combattant, accomplisseur, socialiseur. Le user est un mix avec une composante majeure.
Test psycho pour faire émerger notre profil, sur kahoot.it

A partir de mauvais exemples d'UX dans le jeu vidéo :
- adapter le vocabulaire au user (ex: un cookie sur un navigateur est un gateau sur un bateau pour ma grand-mère)
- respecter les automatismes/conventions
- ne pas compter sur la mémoire du user (ex: comparateur vs 2 pages de caractéristiques)
- adapter les intéractions selon le device (ex: curseur sur console vs PC)
- laisser le choix de la quantité d'informations (densité informationnelle)

Utiliser des outils pour les tests utilisateurs.
Observer les mains, le visage, l'écran, les sons.

Les secrets de Miyamoto (Créateur de Mario, Donkey Kong) : 
- exemple d'ergonomie
- simplicité
- crée de la joie (petite victoire, objectif clair, surprise)
- affordance, autoporteur de sens (ex: <img src="https://upload.wikimedia.org/wikipedia/en/2/21/Goomba2.gif" width="15" alt="Goomba"> a l'air méchant, si <img src="https://i.pinimg.com/originals/78/09/ed/7809ed657b14bdf0f30ca4ab59877bfe.png" width="15" alt="Mario"> regarde à droite, il va à droite)

## l'UX a sauvé mon DEVOPS (REX)

<a href="http://www.youtube.com/watch?feature=player_embedded&v=ovbw8U6NZxI
" target="_blank"><img src="http://img.youtube.com/vi/ovbw8U6NZxI/0.jpg" 
alt="l'UX a sauvé mon DEVOPS" width="240" height="180" border="2" align="right"/></a>

*Estelle Landry & François Teychene - Elium / Saagie*

Comment améliorer la communication entre DEV et DEVOPS (ex-OPS) en s'inspirant des problèmatiques, d'ateliers UX ?
- Faire comprendre que le DEVOPS est l'intégration des OPS, pas une suppression
- Reprioriser (le backlog OPS était trop gros)
- Aligner la road map DEV et OPS (board)
- 5 pourquois : fait émerger les problèmes primaires
- Intéresser les uns aux besoins des autres (pour l'UX, le designer s'intéresse au user)
- S'accorder sur des engagements communs, pas managériaux (6 chapeaux, personas UX)

En conclusion, procéder par étapes, avec les ateliers :
Communication -> Visibilité -> Engagement

A noter une différence entre les DEV qui expriment souvent des solutions, moins un besoin comme un user d'UX.

## Tout le monde sait comment utiliser Angular / React / Vue JS…mais savez-vous comment utiliser JavaScript ?

<a href="http://www.youtube.com/watch?feature=player_embedded&v=PE0GPOtwYkI
" target="_blank"><img src="http://img.youtube.com/vi/PE0GPOtwYkI/0.jpg" 
alt="Tout le monde sait comment utiliser Angular..." width="240" height="180" border="2" align="right"/></a>

*Aurélien Loyer & Nathan Damie - Zenika*

- Savoir où est implémentée une fonctionnalité : typescript vs framework vs javascript (Ecma 5, 6, ...)
- Vanilla JS est un fwk minimum pour du js "pur"
- Tous les frameworks implémentent des fonctionnalités de base qui sont réalisables en vanilla (live code de binding, templating, routing)
- Une fois ces communs implémentés (fwk ou pas), les problématiques émergent et à partir de ce moment le choix du framework intervient

## **Back to back**

## gRPC, communiquons autrement

<a href="http://www.youtube.com/watch?feature=player_embedded&v=6BcfghWezuU
" target="_blank"><img src="http://img.youtube.com/vi/6BcfghWezuU/0.jpg" 
alt="gRPC" width="240" height="180" border="2" align="right"/></a>

*Sébastien FRIESS - SFEIR*

Un peu d'Histoire :
- 1990 HTTP/1
- 1992 CORBA
- 1997 Java/RMI, seulement Java
- 1999 EJB, seulement Java
- 1999 SOAP & WSDL, XML everywhere 
- 2000 HTTP/JSON REST, interopérabilité, a mis du temps à émerger
- 2008 Protocol Buffers
- 2009 Thrift, RPC
- 2015 gRPC

gRPC
- multilangages (10 langages + mobile)
- basé sur HTTP/2
- plugins (retry, ...)
- secure par défaut (TLS)
- open source
- typage fort
- performant grâce au protocol buffers
- numérotation des champs : suppression, ajout transparent et sans versionning des services
- possibilité de générer/exposer du REST depuis gRPC

## HTTP/2 en pratique

<a href="http://www.youtube.com/watch?feature=player_embedded&v=OQiFCOYvwL0
" target="_blank"><img src="http://img.youtube.com/vi/OQiFCOYvwL0/0.jpg" 
alt="HTTP/2" width="240" height="180" border="2" align="right"/></a>

*Alexis Hassler - Sewatech*

Comparaison sur la rapidité d'affichage d'une image entre HTTP/1.1 vs 2

- body + headers compression
- 1.1 = text, 2 = binary
- Server Push (envoi des requêtes au navigateur pour mise en cache et gagner latence)
- HTTPS (h2) ou non (h2c & clear text, non supporté par les navigateurs)
- Multiplexed

Point sur la compatibilité des clients/serveurs HTTP et des langages : certains h2 uniquement, d'autres h2c uniquement, certains nécessitent des versions de Java ou d'OpenSSL spécifiques.

- moins besoin de minification, de limitation des requêtes API
- consomme plus de thread serveur (pas ce problème avec event loop de vert.x vs tomcat)

## Modern API Authentication 101

<a href="http://www.youtube.com/watch?feature=player_embedded&v=259CYnDVHL0
" target="_blank"><img src="http://img.youtube.com/vi/259CYnDVHL0/0.jpg" 
alt="Modern API Authentication" width="240" height="180" border="2" align="right"/></a>

*Léo Unbekandt - Scalingo*

### API Tokens

- Simplicité d'appel
- Surface d'attaque élevée car token dans l'url, donc loggable
- Pas de délégation d'authentification
- Pas de standard, beaucoup de façon de le passer (header custom, basic auth user/mdp, paramètre) 

### OAuth2

- Délégation d'authentification (auth en tant que pour social login)
- Possibilité d'utiliser JWT cryptographiquement signé avec clés publiques/privées
- Gestion de l'expiration 

## L'open-source à la rescousse de mes APIS: comment les sécuriser grâce à Gravitee.io et Keycloak (Live code)

<a href="http://www.youtube.com/watch?feature=player_embedded&v=Lkr3Hok-rfk
" target="_blank"><img src="http://img.youtube.com/vi/Lkr3Hok-rfk/0.jpg" 
alt="Gravitee.io et Keycloak" width="240" height="180" border="2" align="right"/></a>

*David Brassely & Guillaume Gillon - GraviteeSource / Decathlon*

NB : David est un ex-sogeti, ce qui ne gâte rien !

Gravitee, API gateway entre les devices et les services pour manager la sécurisation les APIs.
- sécurité
- ajout d'entêtes CORS
- pilotage des subscribers
- quotas 
- métriques

Associé à Keycloak :
- délégation d'auth
- mire de login
- gestion mot de passe
- compatible JS, Springboot

