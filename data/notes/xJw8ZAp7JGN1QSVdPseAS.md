
# Contrat type: boutons_charge()

## Metadata
### Nom
boutons_charge()

### Responsabilités
retourne l’état du bouton de charge

### Type
logiciel – interface – public/privé

### Références croisées
U.C. recharger_vehicule

### Algorithme
Le bouton de charge doit être réinitialisé par l’utilisateur après consultation. La méthode retourne l’état du bouton et réinitialise l’état à 0.

### Paramètres Entrées/Sorties
- **Sortie :**
0 relâché, 1 appuyé
- **Pré conditions :**
doit-être remis à zéro
- **Post conditions :**
retourne 1 si le bouton a été précédemment appuyé.

## Commentaires / Cas remarquables :
- _generateursave-charger()_ et _generateursave-deconnecter()_: liès à la MEF
- _generateursave-mef()_ : méthode privée pour gérer la MEF
- _boutons-stop_ et _boutons-charge_ doivent être remis à zéro après lecture
- _generateursave _generer_PWM_ : prend en paramètre {OFF, DC, AC_1K, AC_CL} (**Expliquer**)
- _Base_clients_ : authentifier et reprise (pour vérifier que c’est bien le même client)
