# Reponses

## Mission 5

1. Premier commit : dae5040
2. Commits Contact : 9a3358b et e011024
3. Nombre de commits : voir git log
4. Commande graphique : git log --oneline --graph --all
5. Examiner un commit : git show 9a3358b

## Mission 6

git commit --amend -m "Ajout du copyright dans le pied de page"
amend remplace le dernier commit donc il n'y en a qu'un

## Mission 7

git restore index.html
le fichier revient comme au dernier commit

## Mission 8

git reset --soft HEAD~1
les modifs restent car soft touche pas au fichier
git reset --hard HEAD~1 aurait tout supprime

## Mission 9

git revert 0d58321
cree un nouveau commit qui annule
different de la mission 8 car le commit etait deja partage donc on y touche pas

## Mission 11

git cherry-pick 1122aab
id recupere : 1122aab
un merge aurait pris les 3 commits donc pas adapté

## Mission 12

1.0.0 veut dire
1 = version majeure grosses changements incompatibles
0 = version mineure nouvelles fonctionnalites compatible
0 = correctif corrections de bugs

version suivante pour
correction de bug mineur : 1.0.1
nouvelle fonctionnalite compatible : 1.1.0
refonte majeure incompatible : 2.0.0
