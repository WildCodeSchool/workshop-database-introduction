# Base de données

## Atelier 1 - Introduction aux BDD et SQL

#### Introduction

Cet atelier te permettra de découvrir et de manipuler une base de données.
Dans un premier temps, tu utiliseras uniquement le mode CLI ! 
Commence donc par ouvrir ton terminal.

#### La quête du Graal commence
> Rappel : par convention, les noms de bases, tables, champ, doivent être en anglais, au singulier, et en snake_case

![kaamelott](table_ronde.png)

- Créer une Base de données appelée `kaamelott`
- Crée dedans une table `knight`
- Crée dedans les champs :
    - `id` INT (clé primaire, autoincrémentée)
    - `name` VARCHAR(80), NOT NULL
    - `age` INT, NOT NULL

#### Recrutement de chevaliers
Ajoute les chevaliers suivants à l'aide d'une ou plusieurs requêtes (INSERT)
- Arthur 40ans
- Perceval 35 ans
- Lancelot 38 ans
- ... et d'autres si tu le souhaite

#### On fait l'appel
- Récupère la liste des chevaliers (SELECT)
- C'est l'anniversaire de Perceval, modifie son âge en 36ans (UPDATE)
- Affiche uniquement les chevaliers de plus de 37 ans (utilisation de WHERE)

#### Modification de table pas vraiment ronde
- Ajoute un champ `is_dubbed` (est adoubé) de type BOOLEAN et "nullable" (ALTER)
- Passe la valeur de `is_dubbed` à "true" pour tous les chevaliers
- Tu t'aperçois que Perceval n'est pas adoubé, passe uniquement ce chevalier à "false"

#### Au bûcher !

![kaamelott](aubucher.gif)

- Lancelot a quitté la table ronde, supprime le de la table `knight` (DELETE)
- Vide la table des chevaliers sans la supprimer (TRUNCATE)
- Supprime définitivement la table des chevaliers (DROP)

#### OPTION : Continue à manipuler autant que possible
- Créer la table `weapon`
  - `id` INT (clé primaire, autoincrémentée)
  - `name` VARCHAR(50)
- Ajoute, modifie, supprime des armes (ex : épée, arc, lance, catapulte...) 
