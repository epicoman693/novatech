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

## Questions finales

1. la zone de travail c est mes fichiers modifies
   le staging c est ce que je vais mettre dans le prochain commit
   l historique c est tous les commits enregistres

2. parce que on ne casse pas la branche principale et on peut tester separement

3. mission 8 reset annule le commit localement et reecrit l historique
   mission 9 revert cree un nouveau commit et garde l historique intact

4. quand une urgence arrive pendant un travail pas fini (mission 10)

5. parce qu on prend juste le commit utile sans prendre les autres

6. HEAD montre la ou on est dans l historique

7. HEAD~2 c est le commit deux rangs avant

8. un tag donne un nom a une version precis du projet

9. parce qu ils sont plus faciles a comprendre corriger et annuler

10. parce que ce sont des fichiers temporaires ou secrets logs mots de passe
