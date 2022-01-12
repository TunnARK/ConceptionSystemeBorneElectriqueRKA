
## Cas nominal (sans interruption)

|Acteur|Système|
|:---|:---|
|1. Le _client_ insert sa **carte** |2. Le système authentifie l'identité du _client_ |
||3. Le système retourne _OK_ |
||4. Le système déverrouille la **trappe** |
|5. Le _client_ débranche la **prise** |6. Le système met le **voyant prise** à zéro et le **voyant disponible** à vert |

## Cas nominal (avec interruption)

|Acteur|Système|
|:---|:---|
|1. Le _client_ insert sa **carte** |2. Le système authentifie l'identité du _client_ |
||3. Le système retourne _OK_ |
|4. Le _client_ appuit sur le **bouton STOP** |5. Le _véhicule_ fait passer la tension à 9V  |
||6. Le système déverrouille la **trappe** |
|7. Le _client_ débranche la **prise** |8. Le système met le **voyant prise** à zéro et le **voyant disponible** à vert |

## Variante : Carte non valide

|Acteur|Système|
|:---|:---|
|1. Le _client_ insert sa **carte** |2. Le système authentifie l'identité du _client_ |
||3. Le système retourne _Not OK_ |
||4. Le système affiche une erreur au _client_ |

## Hyperliens 

Retour :
- [[Diagramme des Use Cases|BornElec.2-DiagUseCase]]

Vers les autres scénarios :
- [[UC Recharger le véhicule|BornElec.2-DiagUseCase.UC-Recharger]]
- [[UC Charger la batterie|BornElec.2-DiagUseCase.UC-Charger]]
- [[UC Gérer la base de données|BornElec.2-DiagUseCase.UC-Gérer]]

Vers les diagrammes de séquences :
- [[Diag. Séq. UC Recharger le véhicule|BornElec.3-DiagSequences.UC-Recharger]]
- [[UC Charger la batterie|BornElec.3-DiagSequences.UC-Charger]]
- [[UC Reprendre le véhicule|BornElec.3-DiagSequences.UC-Reprendre]]
- [[UC Gérer la base de données|BornElec.3-DiagSequences.UC-Gerer]]