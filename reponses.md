# Reponses — TP final Git (NovaTech)

## Partie 3 — Mission 5 : Analyse du projet

**1. Identifiant court du premier commit :**

`dae5040` (message : "Creation de la page d'accueil NovaTech")

**2. Commit correspondant a l'ajout de la page Contact :**

Deux commits correspondent a cette fonctionnalite (developpee sur la branche
`feature/contact`) :
- `9a3358b` : "Ajout de la page Contact avec nom, e-mail et bouton d'envoi"
- `e011024` : "Ajout des champs sujet et message au formulaire de contact"

**3. Nombre actuel de commits :**

6 commits.

**4. Commande utilisee pour afficher l'historique sous forme graphique :**

```bash
git log --oneline --graph --all
```

- `--oneline` : un commit par ligne (identifiant court + message)
- `--graph` : dessine l'arbre des branches et des fusions
- `--all` : affiche aussi les autres branches

**5. Examen precis d'un commit de la fonctionnalite Contact :**

Commande utilisee :

```bash
git show 9a3358b
```

Resultat : le commit `9a3358b` a ete cree le 8 octobre 2026 par epicoman693.
Il ajoute le fichier `contact.html` (46 lignes) contenant le debut du
formulaire : champs Nom et E-mail et bouton d'envoi.
