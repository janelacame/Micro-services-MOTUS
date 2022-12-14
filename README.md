# Micro-services-MOTUS

Jeu du motus - architecture micro-services

Par BORGET Valentin et JANELA CAMEIJO Alice

## Run le projet
Ouvrir un terminal => aller dans le dossier du projet en utilisant la commande "cd" => écrire "(sudo) docker-compose up".

```diff 
- !!! Pour profiter pleinement de l'expérience, il est conseillé d'activer le son sur son PC.

- !!! Si vous êtes épileptique ou sensible aux flashs, faites attention à la page score. 

+ NOTE : actuellement le motà deviner s'affiche sur la page index.html pour permettre de le deviner plus facilement. 
+ Il est possible d'ajouter "style="display:none"" à la balise ligne 44 du fichier de code pour réellement jouer au jeu.
```

## Règles du jeu du MOTUS
Le joueur doit se connecter au jeu en entrant son login et son mot de passe dans le formulaire de la page **login.html**. Il est ensuite redirigé vers la page **index.html**.

Le joueur est face à un nouveau formulaire. Il connaît la longeur ainsi la 1 ière lettre du mot à deviner.
Il écrit son idée dans le formulaire, la submit et reçoit un retour sur sa proposition.
Une lettre affichée verte est bien placée. Une lettre affichée orange est bien dans le mot à deviner mais mal placée. Une lettre affichée rouge n'est pas dans le mot à deviner.
Le mot à deviner change à chaque actualisation de la page **index.html**.
Un joueur gagne 1 point lorsqu'il devine un mot en entier.

Le score ainsi que des statistiques sont accessibles sur la page **score.html**. 

[![](https://mermaid.ink/img/pako:eNpVUctuwjAQ_BXLl7oS9MghqpAKAcG5vREOlr0kFok3cjYFhPmgfkd_rE5sVLDk1-zMrHb3yhVq4BkvnWwr9pUXloX1sVNoLShiaFmLjvZsOp37GpWsWY2lsQzOpqPOs6UwVsP5raKmfk3qgcye2Bqhsy8UVX4hRvRRsxgTpKx-GcHl7t97H01LIHZCp30uwOoWjY3_ZJPvntAkckC9s1EXrJN5jKkK1DGGVkJh00oHyWw1Mtbi2yhCd3lCN-Lk0JYJ20QvQ78_TpIJTXtns3sVKTif-e0993ootkRGyDqFDvxWjPdjR4Zz2HzCG3CNNDqM6TqinCpooOBZeGo4yL6mghf2FqiyJ_y8WMUzcj1MeN9qSZAbGQbc8Owg6w5uf18roeU)](https://mermaid.live/edit#pako:eNpVUctuwjAQ_BXLl7oS9MghqpAKAcG5vREOlr0kFok3cjYFhPmgfkd_rE5sVLDk1-zMrHb3yhVq4BkvnWwr9pUXloX1sVNoLShiaFmLjvZsOp37GpWsWY2lsQzOpqPOs6UwVsP5raKmfk3qgcye2Bqhsy8UVX4hRvRRsxgTpKx-GcHl7t97H01LIHZCp30uwOoWjY3_ZJPvntAkckC9s1EXrJN5jKkK1DGGVkJh00oHyWw1Mtbi2yhCd3lCN-Lk0JYJ20QvQ78_TpIJTXtns3sVKTif-e0993ootkRGyDqFDvxWjPdjR4Zz2HzCG3CNNDqM6TqinCpooOBZeGo4yL6mghf2FqiyJ_y8WMUzcj1MeN9qSZAbGQbc8Owg6w5uf18roeU)

## Diagrame service d'authentification :
Le micro-service d'authentification est gére en grande partie par le serveur **api_authen.js** port 5000.
[![](https://mermaid.ink/img/pako:eNp1UctuwjAQ_BVrLzmEOpGqXiwVLqg_wDUSWuwNcePYqR9CFPj3OpQ2lQp7mh2NZ3bXJ5BOEQgI9JHISlpr3HscGsty4aj5e3haLsuMtphiRzYTgnUxjqKqjJNoOheieKnrupoEzutPWnHOfx3md5ORcXtteRcHw8RNM1P_kphgxf0s2ZHstaqKMgXyZXED2zEc2IPo723Ynemfr45ozA5lv5ou8lqU0fVky-KB2U6pmXA2L9MG7gnVmzbEzmeW24PXka79n4IFDOQH1Cpf_TS5N5BtBmpAZKioxWRiA429ZGmOcJujlSCiT7SANCqMP58EokUT6PIFdPWV7w)](https://mermaid.live/edit#pako:eNp1UctuwjAQ_BVrLzmEOpGqXiwVLqg_wDUSWuwNcePYqR9CFPj3OpQ2lQp7mh2NZ3bXJ5BOEQgI9JHISlpr3HscGsty4aj5e3haLsuMtphiRzYTgnUxjqKqjJNoOheieKnrupoEzutPWnHOfx3md5ORcXtteRcHw8RNM1P_kphgxf0s2ZHstaqKMgXyZXED2zEc2IPo723Ynemfr45ozA5lv5ou8lqU0fVky-KB2U6pmXA2L9MG7gnVmzbEzmeW24PXka79n4IFDOQH1Cpf_TS5N5BtBmpAZKioxWRiA429ZGmOcJujlSCiT7SANCqMP58EokUT6PIFdPWV7w)

## Diagrame service de score :
Le micro-service de score est gére en grande partie par le serveur **api_score.js** port 4000.
[![](https://mermaid.ink/img/pako:eNp9kT9PwzAQxb9K5MWtUpJIMFmiLAgJBhiyRkKufUlM_SfYF0HV9rtjEyAdWjzdk9-9--luT4STQBgJ8D6CFXCveOe5aWwWn7ISPosejb5ar3M-qNcgnIfiLWQs6xEHVpbaCa57F5DdVFVVBsA6eUqaBwhBOVuj87yDogN8RDALOgbwdJnTaHmqX56LgF7ZTrW7RfqZRiwngNORCWEj5SlCGwoPXD4oDdnhkOSHVwjf-nxA1LE6A3-d4KPQGy62U8tdWs0tzdFtweb0L_AnaopNy8ku5c2WqXnWM8v_zWRFDHjDlYw32qeUhmAPBhrCYimh5aPGhjT2GK18RFfvrCAM_QgrMg6S4-9JCWu5DnD8AvjoqSc)](https://mermaid.live/edit#pako:eNp9kT9PwzAQxb9K5MWtUpJIMFmiLAgJBhiyRkKufUlM_SfYF0HV9rtjEyAdWjzdk9-9--luT4STQBgJ8D6CFXCveOe5aWwWn7ISPosejb5ar3M-qNcgnIfiLWQs6xEHVpbaCa57F5DdVFVVBsA6eUqaBwhBOVuj87yDogN8RDALOgbwdJnTaHmqX56LgF7ZTrW7RfqZRiwngNORCWEj5SlCGwoPXD4oDdnhkOSHVwjf-nxA1LE6A3-d4KPQGy62U8tdWs0tzdFtweb0L_AnaopNy8ku5c2WqXnWM8v_zWRFDHjDlYw32qeUhmAPBhrCYimh5aPGhjT2GK18RFfvrCAM_QgrMg6S4-9JCWu5DnD8AvjoqSc)

## Limites du projet et perspectives d'amélioration :
```diff 
- !!! Il est nécessaire de rentrer 2 fois son login / mot-de-passe pour accéder au jeu.
```

Un système de **reverse proxy** aurait pu être mis en place afin d'augmenter la résilience du projet et sa tolérance aux fautes.

Un système de consultation des logs et de métrcis de perofrmances aurait pû être ajouté afin de monitorer différents micro-services.
