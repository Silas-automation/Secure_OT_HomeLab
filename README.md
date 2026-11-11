# ot-homelab

Lab personnel de cybersécurité industrielle (OT/ICS), construit avec des machines virtuelles et des cartes électroniques, et documenté semaine après semaine.

## Objectif

Reproduire à petite échelle une architecture industrielle (automate, supervision, pare-feu), observer ses faiblesses, puis tester des mesures de protection et mesurer leur effet.

Concrètement, ce lab me sert à :

- comprendre pourquoi des protocoles industriels comme Modbus sont vulnérables (absence d'authentification et de chiffrement) ;
- mettre en place une segmentation réseau et une détection d'intrusion, puis comparer la situation avant et après ;
- décrire le résultat dans le vocabulaire de la norme ISA/IEC 62443 (zones et conduits) ;
- construire un cas d'étude simulé : une ligne d'égrenage de coton simplifiée.

## Pourquoi ce projet

Je suis titulaire d'une licence professionnelle en informatique industrielle et maintenance, et je prépare un master en cybersécurité. Je vise le conseil et l'audit en sécurité des systèmes informatiques et industriels, puis la formation. Ce dépôt garde une trace vérifiable de ce que j'ai réellement fait : chaque expérience a sa fiche, ses captures et ses résultats.

## Environnement

- PC hôte : HP ProBook 450 G3, 12 Go de RAM
- Virtualisation : VMware, 3 machines allumées au maximum
- Systèmes : Linux sans interface graphique (Ubuntu Server ou Debian)
- Matériel : Arduino Mega 2560 et STM32 disponibles ; ESP32 et Raspberry Pi à venir

## Outils prévus

OpenPLC (automate simulé), FUXA (supervision), OPNsense (pare-feu), Suricata (détection), Wireshark, Python, Kali Linux (tests d'attaque, dans le lab uniquement).

## Avancement

| Semaine | Thème         | Livrable                                     | Statut   |
| 1       | Mise en place | README, VM Linux, captures                   | Fait     |
| 2       | Réseaux       | Schéma du réseau virtuel et fiche de capture | À venir  |
| 3       | Linux         | Fiche « durcissement SSH »                   | À venir  |
| 4       | Python        | 2 scripts et bilan du mois 1                 | À venir  |

## Captures
<img width="743" height="711" alt="Image_VM_Démarrage" src="https://github.com/user-attachments/assets/6fea71fd-4e97-47f9-8bef-cf7a1eae7713" />


## Règles du projet

- Tous les tests se font dans ce lab isolé, jamais sur un réseau réel.
- Aucun équipement, aucune donnée et aucun schéma d'une entreprise ne sont utilisés ou publiés.
- Les fichiers des machines virtuelles ne sont pas versionnés : seules les notes, les scripts, les schémas et les captures le sont.
