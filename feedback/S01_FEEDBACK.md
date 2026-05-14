# Rétroaction automatisée -- S01 (Diagnostic fondamental -- NexaMart kickoff)

_Générée le 2026-05-14T22:25:18+00:00 -- Run `20260514T221333Z-7d34bf6a`_

Ce document est produit par un pipeline reproductible (vérification SQL déterministe + analyse LLM du brief et de la déclaration IA). Une revue humaine précède toujours sa publication. **À ce stade expérimental, aucune note ni étiquette de niveau n'est diffusée : l'objectif est purement formatif.**

---

## 1. Vérification automatique de la requête SQL

La requête extraite de votre brief n'a pas pu être validée automatiquement. Quelques pistes constructives ci-dessous pour vous aider à la rendre exécutable et alignee avec la question posée.

_Observation technique : aucun bloc SQL fencé trouvé et extraction LLM échouée_


**Pistes :**
> Aucun bloc ```sql ... ``` détecté. Encadrez votre requête finale dans la section « Preuve » pour fiabiliser l'auto-validation.
> Extracteur LLM : Le brief fourni ne contient aucune requête SQL dans la section Preuve ou ailleurs.

## 2. Rétroaction pédagogique sur le brief

> Le brief soumis est vide ou trop succinct pour évaluer les livrables attendus; il ne contient ni diagnostic, ni preuve SQL, ni recommandations exploitables. Remplissez chaque section (Question CEO, Réponse exécutive, Modélisation, Preuve, Validation, Risques, Recommandation) avec contenu concret et contrôles exécutables avant la prochaine remise.

### Observations par dimension

**Model quality**
- Observation : brief absent ou trop court
- Piste d'amélioration : Décrire le grain (ex. : ligne de commande) et lister les dimensions et mesures clés; justifier pourquoi le schéma permet de répondre à la question CEO.

**Validation quality**
- Observation : brief absent ou trop court
- Piste d'amélioration : Fournir au moins une requête SQL de validation qui calcule le résultat attendu et ajouter 1–2 checks (NULLs, doublons) exécutables.

**Executive justification**
- Observation : brief absent ou trop court
- Piste d'amélioration : Rédiger une réponse exécutive de 150–300 mots en langage décisionnel qui indique la conclusion et la recommandation au CEO.

**Process trace**
- Observation : brief absent ou trop court
- Piste d'amélioration : Ajouter un journal de développement (≥1 commit) et une note IA précisant outils utilisés et validation humaine; documenter décisions clés.

**Reproducibility**
- Observation : brief absent ou trop court
- Piste d'amélioration : Inclure un README minimal et un script check reproducible (DuckDB/SQL) permettant à un pair de reproduire les résultats.

_Quelques points appellent une attention particulière lors de la prochaine itération : brief_trop_court._

## 3. Déclaration d'utilisation de l'IA

> La déclaration fournit un format clair et un exemple concrèt indiquant outil, étape et validation humaine, mais elle ne mentionne pas les limites ou erreurs observées. Fournissez des indications explicites sur la version/modèle utilisé et décrivez systématiquement les limites détectées pour obtenir la note maximale.

**Sujets bien couverts dans votre déclaration :**

- outils utilisés (nom + version/modèle)
- à quelle étape l'IA a été utilisée
- comment la sortie a été validée par l'humain

**Sujets à ajouter ou expliciter pour la prochaine itération :**

- limites ou erreurs observées

## 4. Pistes d'action pour la prochaine itération

- Reprendre la requête de la section « Preuve » pour qu'elle s'exécute sur `db/nexamart.duckdb` et qu'elle produise la forme attendue (voir pistes en section 1).
- Réviser le brief en tenant compte des observations par dimension de la section 2.
- Compléter `ai-usage.md` en y ajoutant : limites ou erreurs observées.

---

## 5. Traçabilité

- **Run ID :** `20260514T221333Z-7d34bf6a`
- **Devoir :** `S01`
- **Étudiant·e :** `citron-citron5`
- **Commit analysé :** `fb0ab79`
- **Audit (côté instructeur) :** `tools/instructor/feedback_pipeline/audit/20260514T221333Z-7d34bf6a/citron-citron5/`
- **Prompts (SHA-256) :**
  - `sql_extractor_system` : `90ee9e277de7a27f...`
  - `rubric_grader_system` : `505f32d1d8319d66...`
  - `ai_usage_grader_system` : `81cb7fdf89bda55a...`
- **Fournisseur (rubrique) :** `openai`
- **Fournisseur (IA-usage) :** `openai` (gpt-5-mini-2025-08-07)

_Ce feedback a été produit par un pipeline automatisé et **revu par l'équipe pédagogique avant publication**. Aucun chiffre ni étiquette de niveau n'est diffusé à ce stade expérimental : l'objectif est uniquement formatif. Ouvrez une issue dans ce dépôt pour toute question._
