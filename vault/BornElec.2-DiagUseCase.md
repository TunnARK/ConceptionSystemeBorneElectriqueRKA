---
id: GvGzqZlo36WrCiLhz4swq
title: 2- Diagramme des Use Cases
desc: ''
updated: 1641904026515
created: 1636961345726
---

## Contexte

|Les acteurs sont|Ils interagissent avec|
|:---|:---|
|le client |la base de données (abonnés)|
|le véhicule|la prise|
|l'opérateur|la gestion et les statistiques de la base de données|
|la borne| l'ensemble materiel pour piloter (les voyants, les boutons, le lecteur, ...)|

Les fonctions principales peuvent être groupées par cas d'utilisation "UC" de la façon suivante :
- **Recharger le véhicule** (incluant charger la batterie et reprendre le véhicule)
- **Gérer la base de données**
- **Configurer la borne**

Dans le cadre de ce mini-projet, nous n'allons pas aborder la partie **UC Configurer la borne**. 

## Diagramme des "Use Cases"

![](/assets/images/DiagUseCase.png)

## Scénario des UC

- [[Scénario de Recharger|BornElec.2-DiagUseCase.UC-Recharger]]
- [[Scénario de Charger|BornElec.2-DiagUseCase.UC-Charger]]
- [[Scénario de Reprendre|BornElec.2-DiagUseCase.UC-Reprendre]]
- [[Scénario de Gérer|BornElec.2-DiagUseCase.UC-Gérer]]

## Hyperliens
 
Retour :
- [[Phase d'Analyse|BornElec.1-PhaseAnalyse]]

Suivant : 
- [[Séquences des Use Cases|BornElec.3-DiagSequences]]