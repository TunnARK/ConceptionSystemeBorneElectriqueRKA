---
id: ehm0Bhn9He4yQnHHK0mcl
title: Scénario Recharger
desc: ''
updated: 1641902643029
created: 1638367646515
---
 
## Cas nominal 

|Acteur|Système|
|:---|:---|
|1. Le _client_ insère sa carte |2. Le système identifie le _client_|
||3. Le système fait clignoter le **voyant charge** de la _borne_ en vert pendant 8 secondes|
|4. Le _client_ a 1min pour appuyer le **bouton charge**|5. Le système éteint le **voyant disponible**|
|6. le _client_ retire sa carte|7. Le système déclanche la charge de la batterie*  |
||8. Le système met le voyant disponible à vert|

*cf. [[Scénario UC Charger la batterie|BornElec.2-DiagUseCase.UC-Charger]]

## Variante 1 : Client inconnu

|Acteur|Système|
|:---|:---|
|1. Le _client_ insère sa carte |2. Le système _client inconnu_|
||3. Le système met le **voyant défaut** à rouge|
|4. Le _client_ retire sa carte||

## Variante 2 : Délai dépassé 

|Acteur|Système|
|:---|:---|
|1. Le _client_ insère sa carte |2. Le système identifie le _client_|
|3. Le système fait clignoter le **voyant charge** de la _borne_ en vert pendant 8 secondes|
|4. Le _client_ a 1min pour appuyer le **bouton charge**|5. Le système détecte que le **bouton charge** n'a pas été appuyé en 1 minute |
|5. Le _client_ retire sa carte||

## Hyperliens 

Retour :
- [[Diagramme des Use Cases|BornElec.2-DiagUseCase]]

Vers les autres scénarios :
- [[UC Charger la batterie|BornElec.2-DiagUseCase.UC-Charger]]
- [[UC Reprendre le véhicule|BornElec.2-DiagUseCase.UC-Reprendre]]
- [[UC Gérer la base de données|BornElec.2-DiagUseCase.UC-Gérer]]

Vers les diagrammes de séquences :
- [[Diag. Séq. UC Recharger le véhicule|BornElec.3-DiagSequences.UC-Recharger]]
- [[UC Charger la batterie|BornElec.3-DiagSequences.UC-Charger]]
- [[UC Reprendre le véhicule|BornElec.3-DiagSequences.UC-Reprendre]]
- [[UC Gérer la base de données|BornElec.3-DiagSequences.UC-Gerer]]