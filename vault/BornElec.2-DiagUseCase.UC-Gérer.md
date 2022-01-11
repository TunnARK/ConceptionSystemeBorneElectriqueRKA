---
id: 3H7c2A8G4FZkApivouiWv
title: Scénario UC Gérer la base de données
desc: ''
updated: 1640784787890
created: 1638368052227
---

## Ajouter un client :

|Acteur(s)|Système|
|:---|:---|
|1. Le _client_ communique à l'_opérateur_ ses **identifiants** ||
|2. L'_opérateur_ demande à la **base de données** si elle est pleine |3. La **base de données** répond non |
|4. L'_opérateur_ crée un nouveau client dans la **base de données** ||
|5. L'_opérateur_ enregistre les **identifiants** du _client_ ||

## Supprimer un client :

|Acteur(s)|Système|
|:---|:---|
|1. Le _client_ demande suppression à l'_opérateur_ ||
|2. L'_opérateur_ sélectionne le _client_ dans la **base de données** ||
|4. L'_opérateur_ déassocie le _client_ de la carte ||
|5. L'_opérateur_ supprime le _client_ de la **base de données** ||

## Associer une carte à un client :

|Acteur(s)|Système|
|:---|:---|
|1. L'_opérateur_ choisit un _client_ ||
|2. L'_opérateur_ vérifie si le _client_ existe dans la **base de données** |3. La **base de données** répond oui |
|4. L'_opérateur_ choisit une carte et vérifie si le **numéro de carte** est disponible |5. La **base de données** répond oui |
|6. L'_opérateur_ associe la carte au client ||

## Déassocier une carte à un client :

|Acteur(s)|Système|
|:---|:---|
|1. L'_opérateur_ choisit un couple (carte, _client_) ||
|2. L'_opérateur_ déassocie la carte du client ||

## Hyperliens 

Retour :
- [[Diagramme des Use Cases|BornElec.2-DiagUseCase]]

Vers les autres scénarios :
- [[UC Recharger le véhicule|BornElec.2-DiagUseCase.UC-Recharger]]
- [[UC Charger la batterie|BornElec.2-DiagUseCase.UC-Charger]]
- [[UC Reprendre le véhicule|BornElec.2-DiagUseCase.UC-Reprendre]]

Vers les diagrammes de séquences :
- [[UC Recharger le véhicule|BornElec.3-DiagSequences.UC-Recharger]]
- [[UC Charger la batterie|BornElec.3-DiagSequences.UC-Charger]]
- [[UC Reprendre le véhicule|BornElec.3-DiagSequences.UC-Reprendre]]
- [[UC Gérer la base de données|BornElec.3-DiagSequences.UC-Gerer]]

