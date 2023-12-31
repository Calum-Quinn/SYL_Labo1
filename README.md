# SYL_Labo1

### Question 1

#### D'après vous, à quoi correspond le *bit de carry* dans un additionneur binaire, et pourquoi est-il important dans l'addition de nombres?

Il sert principalement dans des additioneurs à plus de 1 bit. Lorsque deux bits sont additionés, on regarde s'il y a un carry qui doit être pris en compte pour l'addition des deux prochains bits. Si c'est le cas la prochaine addition aura trois bits à considérer et peut elle aussi avoir un bit de carry qui est à 1 si les bits valent ```1 1 0``` ou ```1 1 1``` (l'ordre des bits ne porte aucune importance).

Exemple: Si on additionne deux 1 en binaire sans le bit de carry ça va nous donner 0 mais par contre si on utilise le bit de carry qui est "additionné au prochain bit" (qui vaut 0) ça nous donnera 10.

<br>

### Question 2

#### A partir de la définition proposée, expliquer ce qu'est un *modular sum* à l'aide d'un schéma ou d'une explication simple.

"*Un `modular sum` se calcule en additionnant les données entre elles sans carry puis en effectuant le complément à deux de ce résultat.*"

Un modular sum représente la formule: `A + B + C = -D` car en binaire le complément à deux représente simplement la négative d'un nombre. Donc pour montrer que l'ordre dans un modular sum n'est pas important on peut faire des transformations basiques pour arriver à la conclusion que `A + B + C + D = 0`.

<br>

### Question 3

#### Quelle est la valeur de checksum attendue pour les constantes définies?

0000 0101 (trouvée à l'aide du Circuit Checksum et vérifié à la main en faisant les calculs)

![Vérification](Verification.png)

<br>

### Question 4

#### Sauvegarder le chronogramme (capture d'écran). Quelles observations peut-on faire?

Export
![Export](Chronogramme.png)

Capture
![Capture](ChronogrammeCapture.png)

On peut voir que les entrées a, b et c sont fixes, car ce sont des constantes. Seulement l'entrée d varie, car c'est un compteur. La sortie est a zéro, sauf pour une valeur (5) de d.

#### Selon quelles conditions la sortie *VerifyIntegrity* passe-t-elle à 1?

La sortie VerifyIntegrity passe à 1 si d correspond au modular sum des entrées a, b et c.
