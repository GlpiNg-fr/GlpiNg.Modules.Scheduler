# GlpiNg.Modules.Scheduler

*[English version](README.en.md)*

Module Planificateur de GlpiNg : lance automatiquement les tâches dont la fenêtre planifiée s'ouvre.

> **Avertissement** — GlpiNg est un projet indépendant. Il n'est ni affilié à, ni approuvé,
> soutenu ou sponsorisé par Teclib' ou le projet GLPI. « GLPI » et « GLPI-Agent » sont des
> marques de leurs propriétaires respectifs ; elles ne sont citées ici que pour décrire la
> compatibilité de GlpiNg avec le protocole GLPI-Agent et l'import depuis une base GLPI.

## Contenu

- Tâches de déploiement
- Tâches réseau
- Tâches Wake-on-LAN
- Actions automatiques (`ICronTask`) exécutées au tick du module Cron, sans boucle de fond propre

## Utilisation

Ce dépôt est un sous-module de [GlpiNg](https://github.com/GlpiNg-fr/GlpiNg), sous
`src/GlpiNg.Modules.Scheduler`. Il ne se compile pas seul : il référence `GlpiNg.Modules.Abstractions`, `GlpiNg.Modules.Deployment` par chemin relatif.

```bash
git clone --recurse-submodules https://github.com/GlpiNg-fr/GlpiNg.git
```

L'hôte l'enregistre par `services.AddSchedulerModule()` (voir `Program.cs`).

## Licence

[GNU Affero General Public License v3.0](LICENSE).
