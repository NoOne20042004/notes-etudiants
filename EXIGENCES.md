# Exigences de sécurité de l'application des notes

| # | Exigence : « Le système doit… » | Vérification | Étape du SDLC | Test |
|---|---|---|---|---|
| 1 | Chercher un étudiant sans que le texte saisi puisse modifier la requête SQL | Test automatique et revue de code | Développement | S1 |
| 2 | Refuser la modification d'une note à toute personne non identifiée (réponse 401) | Test automatique | Conception | S2 |
| 3 | Refuser la modification d'une note à un étudiant (réponse 403) | Test automatique | Conception | S3 |
| 4 | Limiter chaque enseignant aux notes de son propre module (réponse 403) | Test automatique | Conception | S4 |
| 5 | Accepter uniquement une note numérique comprise entre 0 et 20 (réponse 400) | Test automatique | Développement | S5 |
| 6 | Ne montrer aucun détail technique à l'utilisateur en cas d'erreur (réponse 500 générique) | Test automatique | Développement | S7 |
| 7 | Permettre à l'enseignant du module de modifier la note de ses étudiants | Test automatique | Exigences | S6 |