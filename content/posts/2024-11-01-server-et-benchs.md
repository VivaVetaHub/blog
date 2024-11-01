---
title: 'Jour 5 : Tests de Serveur et Outils de Charge pour le Carnet de Santé Numérique'
date: 2024-11-01T20:54:00-00:00
summary: Aujourd’hui, tests serveurs avec Apollo et Rust, exploration d’outils de charge (k6, Siege), et réflexion sur GraphQL vs OpenAPI. De bonnes pistes pour avancer dans le cahier technique !
draft: false
---

# Jour 5 : Tests de Serveur et Outils de Charge pour le Carnet de Santé Numérique

## Introduction

Aujourd'hui, j'ai axé mon travail sur les tests de serveurs en **Rust** avec Apollo et l'exploration de divers outils de test de charge. J'ai aussi approfondi mes recherches sur **GraphQL** et **OpenAPI** pour mieux définir notre approche API. Bien que beaucoup de questions demeurent, ces avancées enrichissent notre **cahier des spécifications techniques**.

## Outils de Test de Charge

Pour évaluer la robustesse de notre serveur, j'ai exploré plusieurs outils :

- **Siege** et **ab** : Simples et rapides à configurer, mais manquant de souplesse. Ils peuvent rester utiles pour des tests basiques.
- **k6** : Belle découverte avec des tests performants. Cependant, le rendu est très orienté cloud, ce qui peut limiter son usage.
- **Yandex**,  **Gatling** et **Thung** : Prometteurs, mais ils nécessiteront des tests plus poussés.
- **SoapUI** et **JMeter** : Ne correspondent pas vraiment aux besoins de notre projet.

Ces outils offrent chacun leurs avantages, mais les essais supplémentaires permettront d'identifier ceux qui sont les mieux adaptés à nos exigences en matière de performance et de flexibilité.

## Tests Serveur et APIs

### Serveur

Les tests se sont également concentrés sur les performances des serveurs en **Rust** et **Apollo** :

- **Serveur Rust Juniper** : Il s'est révélé très performant. Une version avec base de données sera nécessaire pour tester davantage en situation réelle.
- **Serveur Apollo** : J'ai pu intégrer le **codegen** depuis le schéma, une fonctionnalité particulièrement intéressante que j'aimerais conserver pour la suite.

### APIs

J'ai également comparé **GraphQL** et **OpenAPI** pour notre approche API :

- **GraphQL** semble mieux intégré dans l'écosystème actuel de l'application. Cependant, des points sensibles comme la sécurité et le logging demandent encore des clarifications.
- **OpenAPI** a progressé, mais les avantages de GraphQL restent prépondérants pour la flexibilité du projet.

## Conclusion

Ces tests offrent de premiers éclaircissements sur le choix des technologies et des outils. En continuant d'approfondir les solutions de test de charge et les options de serveurs, nous pourrons affiner les décisions techniques et optimiser le **Carnet de Santé Numérique**.
