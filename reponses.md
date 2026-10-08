# Reponses — Mission 5

**1. Identifiant court du premier commit :**

`dae5040` — "Creation de la page d'accueil NovaTech"

**2. Commit de l'ajout de la page Contact :**

Deux commits (developpes sur la branche `feature/contact`) :
- `9a3358b` : "Ajout de la page Contact avec nom, e-mail et bouton d'envoi"
- `e011024` : "Ajout des champs sujet et message au formulaire de contact"

**3. Nombre actuel de commits :**

8 commits.

**4. Commande pour afficher l'historique sous forme graphique :**

```bash
git log --oneline --graph --all
```

**5. Commande pour examiner un commit Contact :**

```bash
git show 9a3358b
```

Ce commit ajoute le fichier `contact.html` (46 lignes) : debut du formulaire
avec Nom, E-mail et bouton Envoyer.

## Partie 4 - Mission 6 : mauvais message de commit

Commande utilisee :

```bash
git commit --amend -m "Ajout du copyright dans le pied de page"
```

amend remplace le dernier commit par un nouveau : il n'y a bien qu'un seul
commit pour cette modification.

## Partie 4 - Mission 7 : modification a abandonner

Commande utilisee :

```bash
git restore index.html
```

Le fichier est revenu exactement a l'etat du dernier commit.

## Partie 5 - Mission 8 : commit local incorrect

Commande choisie :

```bash
git reset --soft HEAD~1
```

Pourquoi les modifications sont toujours presentes : `--soft` annule
seulement le commit, il remet les modifications dans la zone de staging.
Le fichier de travail n'est pas touche.

Methode qui aurait aussi supprime les modifications du fichier :

```bash
git reset --hard HEAD~1
```

`--hard` efface le commit ET les modifications dans le fichier.

## Partie 5 - Mission 9 : commit partage a annuler

Commande utilisee :

```bash
git revert 0d58321
```

Historique apres :

```
78657d3 Revert "Ajout promotion"
0d58321 Ajout promotion
```

Pourquoi c'est different de la mission 8 : ici le commit etait deja partage
avec l'equipe. On ne peut pas le supprimer ni le reecrire (reset ou amend),
car les autres l'ont deja dans leur historique. `revert` cree un NOUVEAU
commit qui fait l'inverse : l'historique reste intact et tout le monde le
voit pareil.
