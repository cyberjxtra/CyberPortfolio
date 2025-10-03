# CyberPortfolio
Portfolio cybersécurité : labs TryHackMe, CTFs et notes

# Lab : Pré‑Security — Principes fondamentaux de Windows

## Objectif

Apprendre et documenter les bases de la sécurité sous Windows : navigation, commandes de base, prise en main d'une machine cible sur TryHackMe et bonnes pratiques.

## Pré‑requis

* Compte TryHackMe
* VM ou accès à la machine TryHackMe du lab
* Connaissances de base : navigation dans un terminal, notions réseau

## Matériel / environnements utilisés

* Plateforme : TryHackMe
* OS cible : Windows (nom de la machine : `THM-Win10`)
* Mon poste : Windows / Linux (indiquer la version)

## Étapes réalisées (déroulé)

1. **Connexion**

   * Connexion à la machine via la méthode indiquée sur TryHackMe (VPN ou navigateur selon le lab).
2. **Reconnaissance initiale**

   * Découverte des services exposés (scan rapide si autorisé : `nmap -sC -sV <IP>`)
   * Vérification de la disponibilité des partages et services Windows (SMB, RDP, HTTP...).
3. **Exploration du système**

   * Récupération d'informations basiques : `whoami`, `hostname`, `systeminfo` (si accessible).
   * Liste des utilisateurs locaux : `net user`.
4. **Exploitation basique / tâches pratiques**

   * Rechercher des fichiers de configuration ou indices (fichiers texte, scripts).
   * Tester l'élévation de privilèges (techniques basiques lorsque le lab le demande).
5. **Nettoyage / sortie**

   * Fermer proprement les connexions et documenter l'état final de la machine.

## Commandes et exemples utiles

* `whoami` — afficher l'utilisateur courant
* `hostname` — afficher le nom de la machine
* `systeminfo` — informations système (si accessible)
* `net user` — lister les utilisateurs locaux
* `nmap -sC -sV <IP>` — scan de découverte (si autorisé par le lab)
* `dir` / `ls` — lister les fichiers

> ⚠️ Toujours respecter les règles du lab : ne pas exécuter de scans agressifs si le lab l'interdit.

## Captures / Preuves (à ajouter)

* Capture 1 : écran de connexion à la machine
* Capture 2 : sortie de la commande `whoami`
* Capture 3 : résultat du scan / service découvert

(Glisser les images dans le repo / dossier `TryHackMe/` sous le même nom que le fichier `.md`.)

## Difficultés rencontrées & solutions

* Exemple : connexion VPN échouée → vérifier token / temps d'expiration et relancer le service VPN.
* Exemple : outil manquant → installer les paquets nécessaires ou utiliser une machine alternative.

## Résultats / flag (si applicable)

* Flag obtenu : `FLAG{exemple}` (remplacer par le flag réel si présent dans le lab)

## Leçons apprises

* Bien documenter chaque commande et résultat.
* Commencer par des commandes non destructrices pour comprendre l'environnement.
* Garder un historique clair (captures + commandes) pour pouvoir justifier tes démarches.

## Prochaines étapes recommandées

1. Finir le parcours **Linux Fundamentals** sur TryHackMe.
2. Faire 2 labs supplémentaires de type Windows (ex : Windows PrivEsc).
3. Commencer des CTFs débutants et rédiger 1 writeup par CTF.

## Références

* TryHackMe — page du lab : [https://tryhackme.com/room/windowsfundamentals](https://tryhackme.com/room/windowsfundamentals)
* Documentation Windows : [https://docs.microsoft.com](https://docs.microsoft.com)

---

*Fichier préparé comme modèle — remplace les sections entre crochets par tes informations personnelles et captures.*
