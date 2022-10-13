# Micro-services-MOTUS
Jeu du motus - architecture micro-services
Par BORGET Valentin et JANELA CAMEIJO Alice

## Run le projet
Ouvrir un terminal
Aller dans le dossier du projet en utilisant la commande "cd"
Ecrire "(sudo) docker-compose up" pour run le projet.

## Règles du jeu du MOTUS
Le joueur doit se connecter au jeu en entrant son login et son mot de passe dans le formulaire de la page **login.html**. Il est ensuite redirigé vers la page **index.html**.

Le joueur est face à un nouveau formulaire. Il connaît la longeur ainsi la 1 ière lettre du mot à deviner.
Il écrit son idée dans le formulaire, la submit et reçoit un retour sur sa proposition.
Une lettre affichée verte est bien placée. Une lettre affichée orange est bien dans le mot à deviner mais mal placée. Une lettre affichée rouge n'est pas dans le mot à deviner.
Le mot à deviner change à chaque actualisation de la page **index.html**.
Un joueur gagne 1 point lorsqu'il devine un mot en entier.

Le score ainsi que des statistiques sont accessibles sur la page **score.html**. 

## Diagrame Mermaid
[![](https://mermaid.ink/img/pako:eNpVUctuwjAQ_BXLl7oS9MghqpAKAcG5vREOlr0kFok3cjYFhPmgfkd_rE5sVLDk1-zMrHb3yhVq4BkvnWwr9pUXloX1sVNoLShiaFmLjvZsOp37GpWsWY2lsQzOpqPOs6UwVsP5raKmfk3qgcye2Bqhsy8UVX4hRvRRsxgTpKx-GcHl7t97H01LIHZCp30uwOoWjY3_ZJPvntAkckC9s1EXrJN5jKkK1DGGVkJh00oHyWw1Mtbi2yhCd3lCN-Lk0JYJ20QvQ78_TpIJTXtns3sVKTif-e0993ootkRGyDqFDvxWjPdjR4Zz2HzCG3CNNDqM6TqinCpooOBZeGo4yL6mghf2FqiyJ_y8WMUzcj1MeN9qSZAbGQbc8Owg6w5uf18roeU)](https://mermaid.live/edit#pako:eNpVUctuwjAQ_BXLl7oS9MghqpAKAcG5vREOlr0kFok3cjYFhPmgfkd_rE5sVLDk1-zMrHb3yhVq4BkvnWwr9pUXloX1sVNoLShiaFmLjvZsOp37GpWsWY2lsQzOpqPOs6UwVsP5raKmfk3qgcye2Bqhsy8UVX4hRvRRsxgTpKx-GcHl7t97H01LIHZCp30uwOoWjY3_ZJPvntAkckC9s1EXrJN5jKkK1DGGVkJh00oHyWw1Mtbi2yhCd3lCN-Lk0JYJ20QvQ78_TpIJTXtns3sVKTif-e0993ootkRGyDqFDvxWjPdjR4Zz2HzCG3CNNDqM6TqinCpooOBZeGo4yL6mghf2FqiyJ_y8WMUzcj1MeN9qSZAbGQbc8Owg6w5uf18roeU)

[![](https://mermaid.ink/img/pako:eNp1UL0OgjAQfhVyk0bUvQOLrsYB3ZqQSg-p6Q-216ghvLsFwsg33X1_yV0PtZMIDAK-I9oaz0o8vTDcZgknrdDSvih2l-vtXrLsOPPTNtKzgWXKSvweWjJ6LfhxXq6EjaNKxurlos_HJlVjWKkJ8WEUVR5D52zAzXal0uOkz-oCyMGgN0LJdG8_ahyoRYMcWBolNiJq4sDtkKwikit_tgZGPmIOsZOClvcAa4QOOPwBrrtlbg)](https://mermaid.live/edit#pako:eNp1UL0OgjAQfhVyk0bUvQOLrsYB3ZqQSg-p6Q-216ghvLsFwsg33X1_yV0PtZMIDAK-I9oaz0o8vTDcZgknrdDSvih2l-vtXrLsOPPTNtKzgWXKSvweWjJ6LfhxXq6EjaNKxurlos_HJlVjWKkJ8WEUVR5D52zAzXal0uOkz-oCyMGgN0LJdG8_ahyoRYMcWBolNiJq4sDtkKwikit_tgZGPmIOsZOClvcAa4QOOPwBrrtlbg)
