# Micro-services-MOTUS
Jeu du motus - architecture micro-services
Par BORGET Valentin et JANELA CAMEIJO Alice

## Run le serveur
Ouvrir un terminal
Aller dans le dossier contenant le fichier de code **api.js** en utilisant la commande "cd"
Entrer "node api.js" pour run le serveur

## Run le HAProxy
Run un deuxième serveur sur un autre numéro de port
Aller dans le dossier contenant le fichier de code **1_simple_proxy** en utilisant la commande "cd"
Entrer [...]

## Run l'application
Ouvrir un navigateur
Entrer "localhost:numPort/index.html

## Règles du jeu du MOTUS
Le joueur doit entrer son login dans le formulaire de la page **login.html** puis est redirigé vers la page **index.html**.

Le joueur est face à un nouveau formulaire. Il connaît la longeuur ainsi la 1 ière lettre du mot à deviner.
Il écrit son idée dans le formulaire, la submit et reçoit un retour sur sa proposition.
Une lettre affichée verte est bien placée. Une lettre affichée orange est bien dans le mot à deviner mais mal placée. Une lettre affichée rouge n'est pas dans le mot à deviner.
Le mot à deviner change à chaque actualisation de la page **index.html**.
Un joueur gagne 1 point lorsqu'il devine un mot en entier.

Le score ainsi que des statistiques sont accessibles sur la page **score.html**. 
