---
id: fIaQokEs2DykNUiTudcYU
title: Scénario de Charger
desc: ''
updated: 1641902537952
created: 1638368017338
---

## Cas nominal 

|Acteur|Système|
|:---|:---|
||1. Le système met le **voyant charge** à rouge|
||2. Le système dévérouille la **trappe** de la **prise**|
||3. Le système génère un **signal contenu** à 12V|
|4. Le _client_  branche la **prise**||
|5. Le _véhicule_ fait chuter la **tension** à 9V||
||6. Le système met le **voyant prise** à vert|
||7. Le système vérouille la **trappe**|
||8. Le système génère un **signal PWM** de 1kHz|
|9. Le _véhicule_ ferme le **contacteur S2**||
|10. Le _véhicule_ fait chuter la **tension** à 6V||
||11. Le système ferme le **contacteur AC**|
||12. Le système génère un **signal PWM** variable|
|13. Le _véhicule_ (i.e. la batterie) fait remonter progressivement la **tension** à 9V||
||14. Le système ouvre le **contacteur AC**|
||15. Le système génère une tension continu|
|16. Le _véhicule_ ouvre le contacteur S2||
||17. Le système met le **voyant charge** à vert|

## Variante 1 : Véhicule déjà chargée

|Acteur|Système|
|:---|:---|
||1. Le système met le **voyant charge** à rouge|
||2. Le système dévérouille la **trappe** de la **prise**|
||3. Le système génère un **signal contenu** à 12V|
|4. Le _client_  branche la **prise**||
|5. Le _véhicule_ fait chuter la **tension** à 9V||
||6. Le système met le **voyant prise** à vert|
||7. Le système vérouille la **trappe**|
||8. Le système génère un **signal PWM** de 1kHz|
|9. Le _véhicule_ ferme le **contacteur S2**||
|! 10. Le _véhicule_ fait chuter la **tension** à **9V**||
||~~11. Le système ferme le **contacteur AC**~~|
||~~12. Le système génère un **signal PWM** variable~~|
|~~13. Le _véhicule_ (i.e. la batterie) fait remonter progressivement la **tension** à 9V~~||
||14. Le système ouvre le **contacteur AC**|
||15. Le système génère une tension continu|
|16. Le _véhicule_ ouvre le contacteur S2||
||17. Le système met le **voyant charge** à vert|

## Hyperliens 
Retour :
- [[Diagramme des Use Cases|BornElec.2-DiagUseCase]]

Vers les autres scénarios :
- [[UC Recharger le véhicule|BornElec.2-DiagUseCase.UC-Recharger]]
- [[UC Reprendre le véhicule|BornElec.2-DiagUseCase.UC-Reprendre]]
- [[UC Gérer la base de données|BornElec.2-DiagUseCase.UC-Gérer]]

Vers les diagrammes de séquences :
- [[UC Recharger le véhicule|BornElec.3-DiagSequences.UC-Recharger]]
- [[UC Charger la batterie|BornElec.3-DiagSequences.UC-Charger]]
- [[UC Reprendre le véhicule|BornElec.3-DiagSequences.UC-Reprendre]]
- [[UC Gérer la base de données|BornElec.3-DiagSequences.UC-Gerer]]

