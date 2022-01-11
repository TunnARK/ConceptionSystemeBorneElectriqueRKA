---
id: jx4ZVDrIXNy4W1R4PCMFI
title: UC-Charger
desc: ''
updated: 1639575100819
created: 1638431691864
---

# Scénario UC Charger la batterie
 
## Cas nominal 

|Acteur|Système|
|:---|:---|
||1. Le système met le **voyant charge** à rouge|
||2. Le système dévérouille la **trappe** de la **prise**|
||Le système génère un **signal contenu** à 12V|
|4. Le _client_  branche la **prise**||
|5. Le _véhicule_ fait chuter la **tension** à 9V||
||6. Le système met le **voyant prise** à vert|
||7. Le système vérouille la **trappe**|
||8. Le système génère un **signal PWM** de 1kHz|
|9. Le véhicule ferme le **contacteur S_2**||
|10. Le véhicule fait chuter la **tension** à 6V||
||11. Le système ferme le **contacteur AC**|
||12. Le système génère un **signal PWM** variable|
|13. Le _véhicule_ (i.e. la batterie) fait remonter progressivement la **tension** à 9V||
||14. Le système ouvre le **contacteur AC**|
||15. Le système génère une tension continu|


*cf. [[UC Charger la batterie|BornElec.2-DiagUseCase.UC-Charger]]

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
- [[UC Gérer la liste|BornElec.2-DiagUseCase.UC-Gérer]]

Vers les diagrammes de séquences :
- [[UC Recharger le véhicule|BornElec.3-DiagSequences.UC-Recharger]]
- [[UC Charger la batterie|BornElec.3-DiagSequences.UC-Charger]]
- [[UC Reprendre le véhicule|BornElec.3-DiagSequences.UC-Reprendre]]
- [[UC Gérer la liste|BornElec.3-DiagSequences.UC-Gerer]]

