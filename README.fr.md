[English](README.md) | [Français](README.fr.md)

# Stations distribuées NeoMundi
## Cadre expérimental de gouvernance, de gestion des données et de contribution

**Statut du dépôt :** cadre public expérimental  
**Phase initiale :** septembre–décembre 2026  
**Version :** 0.1  
**Maintenu par :** NeoMundi Hub

---

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
