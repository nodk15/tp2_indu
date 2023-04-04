# TP2 - Reponses aux questions

## Exercice 1 : GitHub Actions

- Quelles étapes sont réalisées par cette action ?

Cette Action installe les dependances du projet et lance les tests unitaires avec pytest sur un container ubuntu-latest avec python 3.10 pour tester que notre projet fonctionne sur une machine vierge.

- Une étape est définie au minimum par 2 paramètres, lesquels sont-ils et à quoi servent-ils ?

Le paramètre name permet de donner un nom à l’étape. Le paramètre run permet de définir la commande à exécuter.

- La première étape contient un paramètre ‘with’, a quoi sert-il ?

Le paramètre with permet de définir les variables d’environnement pour l’étape. Ici, on définit la version de python à utiliser.

## Exercice 2 : Qualité de code

- Sur l’onglet Summary d’une analyse de code, SonarCloud fournit 4 indicateurs. Quels sont-ils et quelles sont leurs utilités ?

### Reliatbility

Permet de déterminer la fiabilité du code en fonction de la quantité de bugs et de vulnérabilités qui doivent être corrigés.

### Maintainability

Permet de déterminer la facilité de maintenance du code en fonction de la confusion et de la difficulté à maintenair.

### Security

Permet de déterminer la sécurité du code, en fonction des parties de code qui pourrais être exploitées par des attaquants.

### Security Review

Permet de détecter des parties sensible du code potentiellement vulnérables (ex: mot de passe en clair)

- À quoi sert l’indicateur Quality Gate ?

Le Quality Gate est un ensemble de conditions booléennes basées sur des mesures. Il vous permet de savoir immédiatement si votre projet est prêt pour la production. Si votre statut actuel n'est pas "Passé", vous verrez quelles mesures ont causé le problème et les valeurs requises pour passer.


b)

- Quelle est la différence entre les sections New code et Overall Code dans l’onglet Summary ?

La section New code contient les informations sur le code ajouté dans la branche depuis la dernière analyse. La section Overall Code contient les informations sur l’ensemble du code de la branche.

- Y a-t-il des Code Smells ? Si oui, combien et pour quelle(s) raisons(s) ?

Oui, 3 Code Smells :

    - une fonction identique mais pas avec le même nom

    - un argument "deferred" non utilisé dans une méthode

    - un argument "deferred" non utilisé dans uen méthode

- Y a-t-il des Security Hotspots ? Si oui, combien et pour quelle(s)raison(s) ?

Oui, 1, car l'image docker qu'on récupère tourner par défault sur root.

