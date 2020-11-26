# API-gene
Petite API générique en PHP facilement déployable via Ansible
zf201126.1432


<!-- TOC titleSize:2 tabSpaces:2 depthFrom:1 depthTo:6 withLinks:1 updateOnSave:1 orderedList:0 skip:1 title:1 charForUnorderedList:* -->
## Table of Contents
* [Buts](#buts)
* [Problématiques](#problématiques)
* [Moyens](#moyens)
* [Utilisations](#utilisations)
* [Divers](#divers)
  * [Comment récupérer la branche kata-API à Alexandre ?](#comment-récupérer-la-branche-kata-api-à-alexandre-)
* [Sources](#sources)
  * [Kata-API](#kata-api)
  * [Ansible-Alex](#ansible-alex)
<!-- /TOC -->


## Buts
Faire une petit API générique en PHP, facilement déployable via Ansible, afin de pouvoir se construire très facilement un service API pour ses applications.


## Problématiques
Afin de pouvoir très facilement la déployer dans ses projets, il faut que l'on assez générique dans les playbooks d'Ansible.

Par exemple:

**J'aimerai pouvoir avoir deux API's dans mon systèmes de déploiement Ansible-Alex**

* API-covid-calc
* API-bataille-navale

Mais peut-être pas forcément sur le **même serveur** !



## Moyens
...



## Utilisations
...




## Divers

### Comment récupérer la branche kata-API à Alexandre ?
Il faut simplement faire sur un dépôt *vide* ceci:
```
git pull --rebase --autostash https://github.com/TacticsCH/Kata-API tacticsch/php
```

Après résoudre les conflits et faire encore:
```
git rebase --continue
```

Et enfin ne pas oublier de faire un:
```
git push --force
```

## Sources
### Kata-API
https://github.com/TacticsCH/Kata-API/tree/tacticsch/php

https://github.com/ponsfrilus/Kata-API

### Ansible-Alex
https://github.com/TacticsCH/ansible-alex
