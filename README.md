# SYL_Labo1

## Questions

### Question 1

#### D'après vous, à quoi correspond le *bit de carry* dans un additionneur binaire, et pourquoi est-il important dans l'addition de nombres?

### Question 2

#### A partir de la définition proposée, expliquer ce qu'est un *modular sum* à l'aide d'un schéma ou d'une explication simple.

```
Un *modular sum* se calcule en additionnant les données entre elles sans carry puis en effectuant le
complément à deux de ce résultat.
```

### Question 3

#### Quelle est la valeur de checksum attendue pour les constantes définies?

0000 0101 (trouvée à l'aide du Circuit Checksum et vérifié à la main en faisant les calculs)

![Vérification](Verification.png)

### Question 4

#### Sauvegarder le chronogramme (capture d'écran). Quelles observations peut-on faire?

Export
![Export](Chronogramme.png)

Capture
![Capture](ChronogrammeCapture.png)

Il y a un court moment lorsque la sortie du *VerifyIntegrity* est à ```1```.

#### Selon quelles conditions la sortie *VerifyIntegrity* passe-t-elle à 1?

La sortie du *VerifyIntegrity* est à 1 lorsque le compteur atteint la valeur de CheckSum des trois autres entrées.

#### Expliquer votre raisonnement dans le rapport au format *.pdf*.
