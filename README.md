# Missions

Surface de travail humain-agents : tâches, blocages, approbations et preuves (application couche 2, home historique agent-board).

Pour une personne qui travaille avec des agents, qui rencontre du travail d'agents invisible et des validations implicites, ce projet permet de suivre tâches, blocages, approbations et preuves sur une surface commune humain-agents, en produisant un tableau de missions où chaque approbation et chaque preuve est tracée, sans dépendre de : aucune action d'agent sans autorisation vérifiable.

## État du projet

<!-- libre-ai:project-status:begin -->
<!-- Section générée depuis project.v1.yaml — ne pas éditer à la main. -->

- Situation actuelle : L'application Missions (couche de commande fail-closed, autorisation conforme au datalog missions-v1, persistance sur la brique data) est greffée et verte ; l'intégration d'agents réels reste à venir.
- Maturité : usable
- Exposition : spec-published
- Confiance : medium
- Preuves vérifiées le : 2026-07-30
- Avancement : 20 % du périmètre actuellement déclaré

<!-- libre-ai:project-status:end -->

## Vérifier

- `bun install && bun run check` — la chaîne de gates du dépôt, tests inclus.
- La fiche [`project.v1.yaml`](./project.v1.yaml) est l'autorité de l'état du projet ; la section « État du projet » ci-dessus en est générée et un gate de flotte échoue si elles divergent.
- La provenance de chaque chemin migré depuis le hub est tracée dans l'index de migration de `libre-ai/libre-ai` (`ecosystem/migration-index.v1.yaml`).
