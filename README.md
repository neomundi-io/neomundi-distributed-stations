# NeoMundi Distributed Stations
## Experimental Governance, Data Stewardship and Contribution Framework
## Cadre expérimental de gouvernance, de gestion des données et de contribution

**Repository status:** Experimental public framework  
**Initial phase:** September–December 2026  
**Version:** 0.1  
**Maintained by:** NeoMundi Hub

---

# Français

## 1. Objet du dépôt

Ce dépôt documente le cadre expérimental des stations distribuées NeoMundi.

Les stations NeoMundi sont des nœuds de mesure, de recherche appliquée et de contribution. Elles permettent à des contributeurs, chercheurs, opérateurs et infrastructures indépendantes de produire des observations comparables à partir d’une même couche métrologique runtime.

Pendant la phase initiale, les stations ne constituent pas :

- des filiales ;
- des franchises ;
- des entités juridiques autonomes ;
- des représentations commerciales exclusives ;
- des autorités habilitées à engager juridiquement NeoMundi.

Elles fonctionnent sous une bannière commune, avec une gouvernance légère, une attribution explicite et une autonomie progressive fondée sur la mesure, la preuve, l’usage et la confiance accumulée.

## 2. Principe fondateur

NeoMundi construit un réseau distribué de mesure :

- centralisé dans sa cohérence ;
- distribué dans ses contributions ;
- progressif dans son autonomie ;
- ouvert dans ses formes institutionnelles futures.

Le réseau vise à renforcer la visibilité, la légitimité et la crédibilité de la métrologie comportementale des IA par la mesure, la méthode, la réplication, la traçabilité, la correction documentée, la diversité des infrastructures et la transparence des limites.

La forme institutionnelle future reste ouverte. Selon les territoires et les usages, elle pourra prendre la forme d’une structure d’intérêt général, d’une organisation non lucrative, d’une activité commerciale, d’un modèle sous licence, d’une structure hybride ou d’un partenariat local spécifique. Aucune de ces formes n’est présumée à ce stade.

## 3. Périmètre expérimental

La première phase couvre la période de septembre à décembre 2026.

Elle doit permettre d’observer :

- quelles stations deviennent réellement actives ;
- quelles contributions produisent de la valeur ;
- quels usages émergent ;
- quelles responsabilités doivent être distribuées ;
- quelles données doivent être mutualisées ;
- quelles formes de gouvernance sont nécessaires ;
- quels modèles économiques sont adaptés ;
- quelles relations méritent d’être institutionnalisées.

Un bilan collectif est prévu en janvier 2027.

## 4. Rôle du hub NeoMundi

Pendant la phase expérimentale, le hub NeoMundi assure :

- la cohérence du cadre métrologique ;
- la consolidation des méthodes communes ;
- la gouvernance de la marque NeoMundi ;
- la gestion des référentiels communs ;
- la coordination des publications de référence ;
- la conservation de la provenance, des versions et des corrections ;
- la validation des communications institutionnelles ;
- la validation des annonces presse et des partenariats structurants ;
- la consolidation des observations remontées par les stations ;
- la définition des conditions d’accès à l’instrument.

Le hub ne cherche pas à absorber les travaux locaux. Il garantit leur comparabilité, leur traçabilité, leur attribution et leur cohérence avec les frontières de preuve du réseau.

## 5. Rôle des stations

Une station peut notamment :

- conduire des campagnes de mesure ;
- tester une articulation avec une infrastructure locale ;
- reproduire un protocole ;
- proposer une méthode ;
- documenter un cas d’usage ;
- produire une analyse ;
- contribuer à une publication ;
- identifier des partenaires ;
- identifier une opportunité scientifique, institutionnelle ou commerciale ;
- enrichir le corpus longitudinal commun.

Le niveau d’effort reste volontairement léger et proportionné aux disponibilités du contributeur.

> **Effort minimal viable, valeur partagée maximale.**

## 6. Données brutes et espace collaboratif

### 6.1 Principe par défaut

Pendant la phase expérimentale, les données brutes nécessaires à la reproductibilité doivent, par défaut, être déposées dans l’espace collaboratif officiel NeoMundi, hébergé sur l’infrastructure retenue par le hub, notamment l’espace partagé Infomaniak.

Cela peut inclure :

- requêtes, prompts et réponses ;
- sorties intermédiaires ;
- journaux d’exécution et traces ;
- métadonnées et configurations ;
- versions de modèles, prompts et politiques ;
- erreurs et receipts ;
- fichiers de résultats ;
- scripts d’analyse ;
- manifests et hashes ;
- rapports de validation.

### 6.2 Les logs ne suffisent pas nécessairement

L’existence de logs techniques ne garantit pas, à elle seule, un accès futur complet aux données brutes.

Selon l’architecture, les logs peuvent expirer, être échantillonnés, rester partiels, exclure les prompts ou les réponses, être redigés, être accessibles uniquement à certains opérateurs, dépendre d’un fournisseur tiers ou ne pas contenir les versions et artefacts nécessaires à la reproduction.

La conservation des données de recherche doit donc être organisée explicitement et ne pas dépendre uniquement des logs de production.

### 6.3 Plan de collecte explicite

Avant toute exécution, chaque campagne doit définir :

- quelles données sont collectées ;
- qui les collecte ;
- où elles sont stockées ;
- qui peut y accéder ;
- combien de temps elles sont conservées ;
- quelles données peuvent être publiées ;
- quelles données doivent être anonymisées ;
- quelles données restent sous restriction ;
- quels éléments sont nécessaires à la reproduction.

### 6.4 Exceptions au dépôt intégral

Le dépôt centralisé des données brutes ne s’applique que lorsqu’il est juridiquement et contractuellement autorisé, compatible avec la confidentialité, la protection des données, les engagements du partenaire et les exigences de souveraineté ou de sécurité.

Lorsqu’un dépôt intégral n’est pas possible, la station doit fournir, selon le niveau d’autorisation disponible :

- un dataset anonymisé ou minimisé ;
- un extrait représentatif ;
- des métadonnées structurées ;
- un manifest ;
- les hashes des fichiers sources ;
- les résultats dérivés ;
- un protocole d’accès ;
- ou une attestation de conservation locale.

### 6.5 Autorité sur les données

Le stockage dans un espace NeoMundi ne transfère pas automatiquement la propriété des données.

Chaque jeu de données doit préciser son propriétaire, son producteur, son responsable de traitement le cas échéant, ses conditions d’usage, ses restrictions, sa durée de conservation, ses conditions de publication et ses conditions de suppression.

## 7. Structure recommandée de l’espace partagé

```text
/stations
  /station-name
    /00_governance
    /01_protocols
    /02_raw_data
    /03_processed_data
    /04_code
    /05_results
    /06_reports
    /07_publication
    /08_corrections
    /09_licenses_and_consents
```

Chaque campagne doit disposer d’un identifiant unique et d’un manifest minimal.

Exemple :

```text
/stations/cee/2026-09-agent-receipt-validation/
```

## 8. Manifest minimal d’une campagne

Chaque campagne doit documenter au minimum :

- identifiant de campagne ;
- station ;
- contributeurs ;
- date ;
- objectif ;
- protocole ;
- infrastructure utilisée ;
- modèles et versions ;
- paramètres ;
- nombre d’exécutions ;
- fichiers produits ;
- hashes ;
- statut de validation ;
- limites ;
- corrections ;
- autorisations de publication ;
- provenance de chaque composant.

## 9. Propriété intellectuelle et attribution

Chaque contributeur conserve la propriété de ses méthodes, logiciels, validateurs, modèles, jeux de données, documents, cadres, travaux antérieurs et composants développés indépendamment.

La publication sous la bannière NeoMundi ne constitue pas un transfert automatique de propriété.

Toute contribution doit préciser :

- l’auteur ;
- l’organisation éventuelle ;
- la version ;
- la provenance ;
- la licence ;
- les droits accordés au hub ;
- les conditions de réutilisation ;
- l’historique des corrections.

Pour les travaux communs, la propriété, la licence, la maintenance, les revenus et la gouvernance doivent être définis séparément avant tout déploiement commercial.

## 10. Publication et remontée au hub

Les méthodes peuvent être consolidées collectivement.

Les observations et publications de référence remontent au hub afin de permettre la comparaison entre stations, la consolidation longitudinale, la production de datasets communs, la rédaction de papiers, la documentation des articulations, la construction de standards et l’archivage des résultats et corrections.

Toute publication doit distinguer :

- la mesure ;
- l’interprétation ;
- la décision ;
- l’hypothèse ;
- le niveau de preuve ;
- les limites ;
- les résultats corrigés ou remplacés.

## 11. Communication publique

Pendant la phase expérimentale, les éléments suivants doivent être validés par le hub avant publication :

- annonce officielle d’une station ;
- partenariat structurant ;
- communication presse ;
- déclaration institutionnelle ;
- usage commercial de la marque ;
- publication présentant une position globale de NeoMundi ;
- présentation d’un pilote comme preuve de production ;
- attribution d’un rôle officiel de représentation.

Aucune station ni aucun contributeur ne peut, sans autorisation écrite, engager juridiquement NeoMundi, promettre une licence ou un accès, annoncer un partenariat officiel, accorder une exclusivité, représenter un résultat local comme une conclusion globale, présenter un signal comme un verdict ou présenter une hypothèse comme démontrée.

## 12. Autonomie progressive

L’autonomie d’une station ne se décrète pas. Elle se construit par la qualité des mesures, la continuité des contributions, la rigueur méthodologique, la capacité de réplication, la traçabilité, la production d’usages réels, la qualité de la coopération et la confiance accumulée.

Une station pourra progressivement recevoir davantage d’autonomie méthodologique, éditoriale, institutionnelle ou opérationnelle lorsque les preuves d’activité et de fiabilité le justifieront.

## 13. Opportunités commerciales

Une station peut identifier une opportunité commerciale ou institutionnelle.

Dans ce cas :

1. l’opportunité est documentée ;
2. le hub et la station examinent ensemble le montage adapté ;
3. les responsabilités sont définies ;
4. les droits sur l’instrument NeoMundi sont préservés ;
5. les conditions économiques sont établies par écrit.

Le montage peut notamment prendre la forme d’une licence, d’une prestation locale, d’un rôle d’opérateur, d’une intégration, d’un apport d’affaires, d’un partage de revenus, d’un partenariat de recherche ou d’une structure dédiée.

Aucun modèle commercial unique n’est imposé pendant la phase expérimentale. En règle générale, l’instrument ou la couche de mesure NeoMundi reste consommé comme composant identifiable de la solution.

## 14. Réversibilité

Une station peut être suspendue, transformée, renommée, fusionnée ou arrêtée.

Cette décision peut résulter d’une évolution des priorités, d’une activité insuffisante, d’un changement de contexte, d’un désaccord, d’une perte de confiance ou d’une difficulté juridique ou opérationnelle.

L’arrêt d’une station ne constitue pas nécessairement une faute ni un jugement sur les personnes.

En cas d’arrêt :

- les travaux restent attribués ;
- la propriété de chacun est préservée ;
- les publications déjà validées restent archivées ;
- les accès sont révoqués si nécessaire ;
- l’usage futur de la bannière NeoMundi est clarifié ;
- aucune réécriture rétroactive de l’historique n’est autorisée.

## 15. Principe humain

Les œuvres collectives reposent autant sur la qualité des relations que sur la qualité des instruments.

Le facteur humain constitue à la fois leur principale richesse et leur principal risque.

Les contributeurs s’engagent à être dignes de l’instrument de mesure qu’ils développent : précis dans leurs affirmations, transparents dans leurs limites, loyaux dans les attributions, ouverts aux corrections, sobres dans les conflits, responsables dans l’exercice de l’autonomie et respectueux du rythme de chacun.

> **Nous mesurons les systèmes avec rigueur ; nous gouvernons le collectif avec la même exigence.**

## 16. Évolution du cadre

Ce document est expérimental.

Il peut évoluer à partir des retours des stations, des difficultés observées, des besoins de recherche, des contraintes juridiques, des usages commerciaux, des exigences de standardisation et des apprentissages issus de la période septembre–décembre 2026.

Toute modification significative doit être versionnée et documentée.

---

# English

## 1. Repository purpose

This repository documents the experimental framework governing NeoMundi’s distributed stations.

NeoMundi stations are measurement, applied-research and contribution nodes. They enable independent contributors, researchers, operators and infrastructures to produce comparable observations using a shared runtime metrological layer.

During the initial phase, stations are not subsidiaries, franchises, autonomous legal entities, exclusive commercial representatives or authorities entitled to legally bind NeoMundi.

They operate under a common banner with lightweight governance, explicit attribution and progressive autonomy based on measurement, evidence, use and accumulated trust.

## 2. Founding principle

NeoMundi is building a distributed measurement network:

- centralized in its coherence;
- distributed in its contributions;
- progressive in its autonomy;
- open in its future institutional forms.

The network seeks to strengthen the visibility, legitimacy and credibility of behavioral AI metrology through measurement, methodology, replication, traceability, documented correction, infrastructure diversity and transparent limitations.

The future institutional form remains open. Depending on the territory and use case, it may become a public-interest structure, a non-profit organization, a commercial activity, a licensed model, a hybrid structure or a specific local partnership. No such form is presumed at this stage.

## 3. Experimental scope

The initial phase covers September through December 2026.

Its purpose is to observe:

- which stations become active;
- which contributions create value;
- which use cases emerge;
- which responsibilities should be distributed;
- which data should be shared;
- which governance mechanisms are required;
- which economic models are appropriate;
- which relationships deserve institutionalization.

A collective review is planned for January 2027.

## 4. Role of the NeoMundi Hub

During the experimental phase, the NeoMundi Hub is responsible for:

- maintaining coherence of the metrological framework;
- consolidating shared methodologies;
- governing the NeoMundi brand;
- maintaining common reference materials;
- coordinating reference publications;
- preserving provenance, versions and correction history;
- validating institutional communications;
- validating press announcements and strategic partnerships;
- consolidating observations received from stations;
- defining conditions of access to the instrument.

The Hub does not seek to absorb local work. Its role is to guarantee comparability, traceability, attribution and consistency with the network’s evidential boundaries.

## 5. Role of stations

A station may conduct measurement campaigns, test an articulation with a local infrastructure, replicate a protocol, propose a methodology, document a use case, produce an analysis, contribute to a publication, identify partners or opportunities and enrich the shared longitudinal corpus.

The expected workload remains deliberately lightweight and proportional to contributor availability.

> **Minimum viable effort, maximum shared value.**

## 6. Raw data and collaborative workspace

### 6.1 Default principle

During the experimental phase, raw data required for reproducibility should, by default, be deposited in the official NeoMundi collaborative workspace hosted on infrastructure selected by the Hub, including the shared Infomaniak environment.

This may include requests, prompts, responses, intermediate outputs, execution logs, traces, metadata, configurations, model versions, prompt versions, policy versions, errors, receipts, result files, analysis scripts, manifests, hashes and validation reports.

### 6.2 Logs are not necessarily sufficient

The existence of technical logs does not guarantee complete future access to raw research data.

Depending on the architecture, logs may expire, be sampled, be incomplete, exclude prompts or responses, be redacted, be accessible only to specific operators, depend on a third-party provider or omit policies, parameters and artifacts required for reproduction.

Research-data preservation must therefore be explicitly organized and must not rely solely on production logs.

### 6.3 Explicit collection plan

Before execution, each campaign must define:

- which data will be collected;
- who will collect it;
- where it will be stored;
- who may access it;
- how long it will be retained;
- which data may be published;
- which data must be anonymized;
- which data must remain restricted;
- which elements are required for reproduction.

### 6.4 Exceptions to complete deposit

Centralized deposit of raw data applies only where it is legally and contractually authorized and compatible with confidentiality, data protection, partner commitments and sovereignty or security requirements.

Where complete deposit is not possible, the station should provide an anonymized or minimized dataset, a representative sample, structured metadata, a manifest, hashes of source files, derived results, an access protocol or a statement confirming local preservation.

### 6.5 Authority over data

Storage in a NeoMundi workspace does not automatically transfer data ownership.

Each dataset must identify its owner, producer, controller where applicable, permitted uses, restrictions, retention period, publication conditions and deletion conditions.

## 7. Recommended shared-space structure

```text
/stations
  /station-name
    /00_governance
    /01_protocols
    /02_raw_data
    /03_processed_data
    /04_code
    /05_results
    /06_reports
    /07_publication
    /08_corrections
    /09_licenses_and_consents
```

Each campaign should have a unique identifier and a minimal manifest.

Example:

```text
/stations/cee/2026-09-agent-receipt-validation/
```

## 8. Minimal campaign manifest

Each campaign must document at least:

- campaign identifier;
- station;
- contributors;
- date;
- objective;
- protocol;
- infrastructure;
- models and versions;
- parameters;
- number of executions;
- generated files;
- hashes;
- validation status;
- limitations;
- corrections;
- publication authorizations;
- component provenance.

## 9. Intellectual property and attribution

Each contributor retains ownership of their methods, software, validators, models, datasets, documents, frameworks, pre-existing work and independently developed components.

Publication under the NeoMundi banner does not automatically transfer ownership.

Each contribution must identify its author, organization where applicable, version, provenance, license, rights granted to the Hub, reuse conditions and correction history.

For joint work, ownership, licensing, maintenance, revenue and governance must be defined separately before commercial deployment.

## 10. Publication and reporting to the Hub

Methods may be consolidated collectively.

Reference observations and publications are reported to the Hub to enable cross-station comparison, longitudinal consolidation, production of common datasets, research papers, articulation documentation, standards development and archival of results and corrections.

Every publication must distinguish measurement, interpretation, decision, hypothesis, evidence level, limitations and corrected or superseded results.

## 11. Public communication

During the experimental phase, official station announcements, strategic partnerships, press communications, institutional statements, commercial use of the brand, global NeoMundi positions, production claims and official representative roles require Hub validation.

Without written authorization, no station or contributor may legally bind NeoMundi, promise a license or access, announce an official partnership, grant exclusivity, present a local result as a global conclusion, present a signal as a verdict or present a hypothesis as demonstrated.

## 12. Progressive autonomy

A station’s autonomy is not declared. It is built through measurement quality, continuity of contribution, methodological rigor, replication capacity, traceability, production of real use cases, quality of cooperation and accumulated trust.

A station may progressively receive greater methodological, editorial, institutional or operational autonomy when evidence of activity and reliability justifies it.

## 13. Commercial opportunities

A station may identify a commercial or institutional opportunity.

In that case:

1. the opportunity is documented;
2. the Hub and station jointly assess the appropriate structure;
3. responsibilities are defined;
4. rights over the NeoMundi instrument are preserved;
5. economic terms are agreed in writing.

The structure may include a license, local service, operator role, integration, referral, revenue sharing, research partnership or dedicated entity.

No single commercial model is imposed during the experimental phase. As a general principle, the NeoMundi instrument or measurement layer remains an identifiable component consumed by the resulting solution.

## 14. Reversibility

A station may be suspended, transformed, renamed, merged or discontinued because of changing priorities, insufficient activity, a change of context, disagreement, loss of trust or legal or operational constraints.

Ending a station does not necessarily constitute fault or a judgment on the people involved.

When a station ends, prior work remains attributed, ownership is preserved, validated publications remain archived, access is revoked where necessary, future use of the NeoMundi banner is clarified and no retroactive rewriting of history is permitted.

## 15. Human principle

Collective work depends as much on the quality of relationships as on the quality of instruments.

The human factor is both its greatest strength and its greatest risk.

Contributors commit to being worthy of the measurement instrument they are building: precise in their claims, transparent about limitations, loyal in attribution, open to correction, restrained in conflict, responsible in the exercise of autonomy and respectful of each person’s pace and contribution.

> **We measure systems rigorously; we govern the collective with the same standard.**

## 16. Evolution of the framework

This document is experimental.

It may evolve based on station feedback, observed difficulties, research needs, legal constraints, commercial use cases, standardization requirements and lessons learned during September–December 2026.

All significant changes must be versioned and documented.
