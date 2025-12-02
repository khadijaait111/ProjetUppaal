README — Modélisation et Vérification d’un SOC avec UPPAAL
## Description du projet

Ce projet consiste à modéliser et vérifier formellement le comportement d’un Security Operation Center (SOC) confronté à un attaquant réel.
L’objectif est de garantir que le système :

détecte correctement les attaques

évite les faux positifs

applique les sanctions adéquates

reste cohérent même face à des événements simultanés

et ne tombe jamais dans un scénario bloquant.

Le projet utilise UPPAAL, un outil de modélisation de systèmes temps-réel, pour représenter les interactions entre l’attaquant, les deux modules SOC, et le Firewall.

## Architecture du modèle

Le système est composé de quatre automates indépendants :

Attaquant : génère des scans, des échecs de login utilisateur et des attaques administrateur.

SOC Scan : détecte les scans rapides dans une courte fenêtre de temps.

SOC Login : analyse les échecs de connexion et vérifie si la cible est un administrateur.

Firewall : applique les sanctions (blocage temporaire ou bannissement définitif).

## Auteurs :
   Khadija AIT YOUSSEF
   Yassine EL IDRISSI
