---
title: Projet Pomodoro
description: ''
position: 1
category: ''
---

## Descriptif
Un système de gestionnaire de tâche et de temps, le principe résumé au plus simple est le suivant:

Gérer vos tâches quotidiennes en les ajoutant via l'interface web, celles-ci peuvent avoir les statuts suivants : TODO, IN PROGRESS, DONE et ARCHIVED.

Vous pouvez bien entendu, les nommées, rajouter des deadlines ainsi qu'une description.

Concernant la gestion de temps, l'application applique le principe de la méthode pomodoro ([https://doc.pomodoro.seelo.ch/pomodoro/concept](https://doc.pomodoro.seelo.ch/pomodoro/concept)), vous effectuez une session composée (de base) de :
5 période de 25 minutes de travail (intensif), séparé par 5 minutes de pauses entre chacune et la dernière pause, est la grande, 15 minutes.

Une fois ces étapes terminées, vous avez effectué une session.

Pour créer une session, il suffit soit de :

1. Cliquer sur la bulle bleue dans la sidebar qui affiche Start session
1. Cliquer sur l'icône expand dans la sidebar et une fois la fenêtre ouverte, cliquer sur le bouton Start session

Vous pouvez interagir les étapes durant votre session, vous pouvez:

- Mettre pause (seulement possible durant une étape en cours)
- Relancer (seulement possible durant une étape en pause)
- Skipper une étape (seulement possible durant une étape en pause)
- Abort l'entier de la session (seulement possible durant une étape en pause)Nous utilisons les websockets pour pouvoir bénéficier d'un affichage/changements des informations en temps réel, les données transmisespar Websocket concernent:Les tâches, (update, delete, create)La session en cours, ainsi que toutes les actions qui vont avec.

## Personnalisation de l'expérience
Vous avez également accès un panel settings, ou vous aurez accès aux informations suivantes:

#### Paramètres généraux
- Changement de l'affichage de l'heure sur l'application (12H/24H)
- Changement du thème (Light, Dark, avec une préférence pour le Dark)
- Changement de votre configuration sélectionnée pour vos sessions

#### Paramètres compte utilisateurs
- Changement de votre Nom, Email et Password

#### Paramétrage de votre session pomodoro
Vous avez les paramètres de session par défaut, vous pouvez choisir de créer une configuration et l'utiliser si vous souhaitez personnaliser vos sessions.

Pour le moment vous pouvez modifier les propriétés suivantes :
- Temps par pomodoro
- Temps pour les petites pauses
- Temps pour les grandes pauses
- Le nombre de pomodoro (étapes de travail) que vous souhaitez effectuer par session.

#### Paramétrage de votre abonnement
Si vous n'êtes pas premium, vous n'aurez accès qu'à la tab Current subscription, qui affiche votre statut de Freemium, ainsi que la limitation appliquée concernant votre statut.

Après avoir upgrade votre statut, vous aurez accès aux informations détaillées relatives à votre abonnement, vous verrez donc apparaître les 4 autres tabs restantes.

## Fonctionnalité Premium et Freemium

La version non payante a une limite de création de 5 tâches. Les utilisateurs premium bénéficient d'un nombre illimité de création de tâches.
**Si vous décidez de révoquer votre abonnement, vous serez toujours bénéficiaire des fonctionnalités premium durant un mois depuis votre précédent paiement**

#### Devenir Premium
- Cliquer sur l'icône Settings en haut à droite de l'application, naviguer dans la tab Subscription et appuyer sur le bouton Upgrade
- Vous allez être redirigé sur la page pour gérer votre abonnement.
- Pour le paiement nous utilisons Stripe

Pour faire un paiement sans la 3D Secure :

- Carte: 4242 4242 4242 4242
- Exp: xx/2022
- Cvc: any

Pour lancer le processus avec 3D Secure (validation 2 étapes)
- Carte: 4000 0027 6000 3184
- Exp: xx/2022
- Cvc: any

Pour plus d'informations sur les cartes de tests : https://stripe.com/docs/testing


## Parcourir le projet
Pour tester le bon fonctionnement vous pouvez vous rendre sur ce lien: [http://front-pomodoro.seelo.ch/](http://front-pomodoro.seelo.ch/)

Vous pouvez soit créer un compte via:[http://front-pomodoro.seelo.ch/register](http://front-pomodoro.seelo.ch/register)

Ou utiliser un compte déjà créé :
- Email: dario.regazzoni@seelo.ch
- Password: Test1234

Vous aurez accès à l'interface frontend de l'application, donc créer des tâches, lancer une session, paramétrer vos préférences, ainsi que voir les informations relatives à votre abonnement.

Pour voir l'interface backend (gérer son abonnement directement):[http://back-pomodoro.seelo.ch/login](http://back-pomodoro.seelo.ch/login)

## Installation en locale (déconseillée)
- Procédure pour installer le backend: [https://doc.pomodoro.seelo.ch/backend/installation](https://doc.pomodoro.seelo.ch/backend/installation)
- Procédure pour installer le frontend: [https://doc.pomodoro.seelo.ch/frontend](https://doc.pomodoro.seelo.ch/frontend)

## Codebases
- Backend: [https://gitlab.com/seelo/pomodoro/backend](https://gitlab.com/seelo/pomodoro/backend)
- Frontend: [https://gitlab.com/seelo/pomodoro/frontend](https://gitlab.com/seelo/pomodoro/frontend)
- Documentation: [https://gitlab.com/seelo/pomodoro/documentation](https://gitlab.com/seelo/pomodoro/documentation)
- Api-documentation: [https://documenter.getpostman.com/view/3290889/TzXzCc15](https://documenter.getpostman.com/view/3290889/TzXzCc15)

## Application live
- Backend: [http://back-pomodoro.seelo.ch/login](http://back-pomodoro.seelo.ch/login)
- Frontend: [http://front-pomodoro.seelo.ch/](http://front-pomodoro.seelo.ch/)
- Documentation: [https://doc.pomodoro.seelo.ch/](https://doc.pomodoro.seelo.ch/)

