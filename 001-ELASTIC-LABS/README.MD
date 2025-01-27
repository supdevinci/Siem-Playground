
# Projet de TP : Configuration d'un laboratoire de surveillance de la sécurité avec Elastic SIEM et Kali Linux

## Résumé Exécutif
Ce projet vise à établir un laboratoire pratique de surveillance de la sécurité en utilisant Elastic SIEM et une machine virtuelle (VM) Kali Linux. L'objectif est de démontrer l'intégration d'Elastic SIEM pour la surveillance en temps réel, la détection des menaces et la visualisation des événements de sécurité à partir des données transférées depuis une VM Kali. En configurant ce laboratoire, le projet fournit un environnement pratique et économique pour améliorer les compétences en cybersécurité, permettant ainsi une détection et une réponse efficaces aux incidents de sécurité.

## Objectifs du Projet
- Configurer Elastic SIEM pour la surveillance de la sécurité avec un compte Elastic Cloud d'essai gratuit.
- Déployer et configurer une VM Kali Linux pour le transfert de journaux et la simulation de menaces.
- Intégrer l'Elastic Agent pour collecter et transférer les événements de sécurité depuis la VM vers le SIEM.
- Simuler des événements de sécurité à l'aide d'outils comme Nmap pour générer des données significatives pour l'analyse.
- Créer des tableaux de bord et des alertes dans Elastic SIEM pour visualiser et surveiller les incidents de sécurité.
- Fournir un guide étape par étape pour la réplication, permettant l'évolutivité du laboratoire pour un usage plus large.

## Méthodologie

### Phase de Configuration :
- Inscription sur Elastic Cloud et déploiement d'une instance Elasticsearch.
- Téléchargement et installation de Kali Linux sur VirtualBox ou VMware.

### Phase d'Intégration :
- Installer l'Elastic Agent sur la VM Kali et le configurer pour transférer les journaux vers le SIEM.
- Vérifier l'ingestion réussie des données à l'aide de requêtes simples dans Elastic SIEM.

### Génération d'Événements :
- Simuler des attaques à l'aide de Nmap et analyser les journaux dans Elastic SIEM.

### Visualisation des Données :
- Créer un tableau de bord pour suivre les tendances des événements de sécurité.

### Création d'Alerte :
- Configurer des alertes pour des incidents de sécurité spécifiques, tels que les analyses Nmap.

## Calendrier du Projet

| Nom de la Tâche                     | Date de Début | Durée     |
|-------------------------------------|---------------|-----------|
| Configuration du Compte Elastic Cloud | 2024-11-20    | 2 heures   |
| Installation de Kali Linux          | 2024-11-22    | 2 heures   |
| Configuration de l'Elastic Agent    | 2024-11-27    | 2 heures   |
| Simulation d'Événements             | 2024-11-30    | 2 heures   |
| Création du Tableau de Bord         | 2024-12-04    | 2 heures   |
| Tests et Documentation              | 2024-12-11    | 4 heures   |

## Ressources Nécessaires

### Matériel :
- Ordinateur portable ou PC avec suffisamment de puissance processeur et RAM (ressource existante).

### Logiciels :
- Elastic Cloud (Essai gratuit) ou via Docker Compose
- VirtualBox ou VMware (Gratuit).
- VM Kali Linux (Gratuit).

## Calendrier du Projet avec Tâches Détaillées

1. **Configuration du Compte Elastic Cloud **
   - Créer un compte Elastic Cloud à l'aide d'une adresse e-mail valide.
   - Déployer une instance Elasticsearch et Kibana en choisissant une configuration d'essai gratuite.
   - Configurer les paramètres de base, comme les régions et les ressources attribuées.
   - Noter les identifiants et URL de l'instance pour la connexion future.

2. **Installation de Kali Linux **
   - Télécharger l'image ISO de Kali Linux depuis le site officiel.
   - Installer Kali Linux sur VirtualBox ou VMware avec une configuration matérielle minimale de 2 CPU et 4 Go de RAM.
   - Configurer le réseau de la VM en mode NAT ou Ponté pour assurer la connectivité.
   - Mettre à jour le système Kali Linux et installer les paquets de base (e.g., Nmap, Netcat).

3. **Configuration de l'Elastic Agent **
   - Télécharger l'Elastic Agent compatible avec Kali Linux depuis l'instance Kibana.
   - Installer l'agent sur la VM Kali en suivant les instructions officielles Elastic.
   - Configurer l'agent pour transmettre les journaux système (e.g., journaux Syslog) à l'instance Elasticsearch.
   - Tester la connexion entre l'agent et le SIEM en vérifiant l'ingestion des premières données.

4. **Simulation d'Événements **
   - Exécuter des scans Nmap depuis Kali Linux pour simuler des activités malveillantes.
   - Générer des journaux de connexion SSH avec des tentatives répétées (e.g., brute force).
   - Observer l'apparition des événements simulés dans Elastic SIEM.

5. **Création du Tableau de Bord **
   - Identifier les métriques clés à surveiller (e.g., IP suspectes, volumes de logs).
   - Créer des visualisations Kibana (e.g., histogrammes, heatmaps) pour analyser les tendances.
   - Construire un tableau de bord complet pour surveiller les menaces en temps réel.

6. **Tests et Documentation**
   - Tester le laboratoire pour assurer le bon fonctionnement de toutes les étapes.
   - Rédiger une documentation détaillée avec des captures d'écran pour chaque étape.
   - Fournir des recommandations pour l'optimisation et l'évolution du laboratoire.

