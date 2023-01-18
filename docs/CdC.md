# Cahier des charges
Ce cahier des charges comprend 3 sous-projets:
1. Tablero: l'éditeur de dashboard.
2. Caliente: un widget de monitorage de température du CPU.
3. Une librairie commune permettant de faire la communication entre le dashboard et les widgets, ou entre widgets.

## Tablero
Tablero est un éditeur de dashboard et est l'application principale.
Ce dernier est une grille de 12 colonnes et 6 lignes, et sera initialement uniquement pour desktop (ratio 16:9).
Il contient 2 modes:
- Mode *Edition*: permets d'ajouter, retirer et déplacer des widgets au sein de la grille.
- Mode *Présentation*: permets de visualiser le dashboard et d'interagir avec les widgets.

### Mode Édition
Un toolbox sur la gauche apparait, et le dashboard sur la droite garde le ratio de l'écran.
Il est possible de grag-&-drop des widgets de la toolbox vers la grille.
Les widgets, une fois sur la grille, peuvent être supprimés ou déplacés, mais un widget ne peut pas être au-dessus d'un autre.
Un widget peut prendre plus d'une case de la grille

### Mode Présentation
Il est possible d'interagir avec les widgets comme mentionné plus loin, mais il n'est pas possible de changer le layout du dashboard.

## Caliente
Caliente est un widget permettant d'afficher en temps réel la température du CPU.
Ce widget peut être personnalisable avec ces paramètres:
1. Température d'un core ou de la moyenne des core à afficher
2. Unité (°C ou °F)
3. Temps de rafraichissement de la valeur