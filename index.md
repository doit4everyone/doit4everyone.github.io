---
title: "DoIt4Everyone - Documentation et procédures : Shadow AI, Microsoft Purview, UTMStack pour PME Suisse"
description: "Guides et procédures techniques gratuits pour PME suisses : gouvernance Shadow AI Microsoft 365, Microsoft Purview, conformité nLPD, DLP, MDCA, DSPM for AI, UTMStack SIEM."
---

<style>
  /* 1. On cache le header et le footer du thème */
  header, footer { display: none !important; }

  /* 2. On réinitialise le conteneur principal pour le centrage et la typographie */
  .wrapper {
    max-width: 900px !important;
    margin: 0 auto !important;
    float: none !important; 
    position: relative !important;
    padding: 40px 20px !important;
    
    /* Typographie moderne et lisible */
    font-family: "Helvetica Neue", Helvetica, Arial, sans-serif !important;
    font-size: 1.1em !important;
  }

  /* 3. On force la section de texte à prendre toute la largeur */
  section {
    width: 100% !important;
    float: none !important;
    margin: 0 !important;
    padding-top: 0 !important;
  }

  /* Centrage des titres principaux */
  h1, h2 { text-align: center; }
</style>

<h1 style="text-align: center;">DoIt4Everyone</h1>

<h2 style="text-align: center;"><strong>Documentation, procédure technique & Guides de lab pour PME Suisse 🇨🇭</strong></h2>

Ce portail centralise des **documentations techniques et des procédures techniques actionnables**, issues de tests en environnements réels, couvrant la sécurité, l'infrastructure et la conformité des systèmes d'information.

Chaque guide est conçu pour être déployé en autonomie, sans dépendre systématiquement d'intervenants tiers.

---

## ✅ Guides disponibles

### 🛡️ Microsoft Purview, gouvernance & nLPD Suisse

**[🔐 Configuration Microsoft Purview 2026](https://doit4everyone.github.io/microsoft-purview-configuration-2026-nLPD/)**
*Procédure de configuration complète de Microsoft Purview pour PME suisses.*

DLP, classification, auto-labelling, gouvernance Copilot, DSPM for AI — sans licence E5.

**En bonus:**
    Une procédure de préparation du tenant pour le POC.
    Des fichiers de démonstration, société Axonix SA (données fictives).

    
> *Vous pourrez notamment y constater que la sécurité et la conformité ne sont pas des problèmes de licence, mais des problèmes d'architecture et de gouvernance.*

<br>

**[🛡️ Gouvernance Shadow AI — Microsoft 365](https://doit4everyone.github.io/shadow-ai-governance-microsoft-365-nLPD/)**
*Guide complet de détection, blocage et gouvernance des usages IA non maîtrisés pour PME suisses.*

MDCA, Purview DLP, DLP inline Edge for Business, DSPM for AI, Insider Risk Management, gouvernance Power Platform — conformité nLPD (art. 5, 6, 8, 9, 16, 19, 24, 62).

**En bonus :**
    Matrice des angles morts avec couverture et efficacité estimée par vecteur.
    Chronologie de déploiement en 4 semaines sans interruption de service.

> *Cette architecture reflète un niveau de contrôle réaliste basé sur les capacités actuelles de Microsoft 365, et non une couverture exhaustive du Shadow AI.*

<br>

**[⚡ Guide MVC Microsoft Purview 2026](https://doit4everyone.github.io/Configuration-Purview-PME-Suisse-nLPD/)**
*Procédure de déploiement Minimum Viable de Conformité (MVC) pour PME suisses.*

2 étiquettes, DLP Exchange, rétention automatique, Break-glass RMS — déploiement en **4 à 6 heures**.

Inclut des adaptations sectorielles pour fiduciaires, architectes, avocats, agences de communication et cabinets médicaux.

---

## 🔐 Sécurité & SIEM — Lab

**[🛡️ UTMStack Lab v11.2.8 — Guide de déploiement](https://doit4everyone.github.io/utmstack-lab/)** *Déploiement complet UTMStack Community Edition pour PME suisses.*

Installation VMware, intégration Suricata (OPNsense), CrowdSec, dashboards OpenSearch et automatisation SOAR.

**En bonus :** Architecture pipeline syslog-ng complète. Règles Suricata custom anti-Mirai. Ban automatique des IPs malveillantes via playbooks SOAR → CrowdSec. Audit NTLM via Windows Event Forwarding en préparation de la migration vers Kerberos (Windows Server 2025).
> *Un lab opérationnel de détection et réponse aux menaces, avec corrélation Threat Intelligence ThreatWinds et géolocalisation des attaquants.*

## ⚠️ Projet en cours de documentation
Ce lab représente plusieurs semaines de travail terrain. La documentation sera publiée progressivement, au fil du temps disponible. Les guides déjà disponibles sont opérationnels et testés en environnement réel.

---

## 🧩 Tips & Notes techniques

**[🔓 Tips & Notes techniques — Lab](https://doit4everyone.github.io/tips-lab/)** *Correctifs et retours d'expérience ponctuels, issus de tests en environnement réel.*

Des blocages rencontrés en laboratoire, leurs causes réelles, les solutions qui fonctionnent — sans détour théorique. Rubrique courte, alimentée au fil des découvertes de terrain.

**Premier tip :** [🔓 VMware Workstation bloqué par VBS/UEFI](https://doit4everyone.github.io/tips-lab/docs/01-vmware-vbs-uefi.html) — débloquer la virtualisation imbriquée sur un PC Secured-core récent.

> *Contrairement aux guides complets ci-dessus, ces notes n'ont pas de roadmap : une page, un problème, une solution testée.*

---

## 🛠️ Travaux en cours

De nouvelles ressources seront publiées au fil des tests de lab et des études, sur des sujets variés liés à la sécurité et à l'infrastructure des SI.

---

## ☕ Soutenir le projet

Ces guides représentent des dizaines d'heures de tests en environnements réels, des frais fixes de licences et d'infrastructure. 

Si ces ressources vous font gagner du temps, vous pouvez contribuer à l'avancée de mes travaux de lab. Merci.

👉 [![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/R5R31YHNIB)

---

ℹ️ *Références, structuration et aide à la rédaction assistées par IA, avec validation humaine finale.*
