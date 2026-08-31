---
title: "DoIt4Everyone - Documentation et procédures : Shadow AI, Microsoft Purview, UTMStack pour PME Suisse"
description: "Guides et procédures techniques gratuits pour PME suisses : gouvernance Shadow AI Microsoft 365, Microsoft Purview, conformité nLPD, DLP, MDCA, DSPM for AI, UTMStack SIEM, AiTM protection WHfB FIDO2."
---

<style>
  header, footer { display: none !important; }
  .wrapper {
    max-width: 900px !important;
    margin: 0 auto !important;
    float: none !important; 
    position: relative !important;
    padding: 40px 20px !important;
    font-family: "Helvetica Neue", Helvetica, Arial, sans-serif !important;
    font-size: 1.1em !important;
  }
  section {
    width: 100% !important;
    float: none !important;
    margin: 0 !important;
    padding-top: 0 !important;
  }
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

**En bonus :**
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

**[⚡ Bundle MVC nLPD — Microsoft 365 Business Premium](https://doit4everyone.github.io/mvc-nlpd-m365/)**
*Quatre guides de conformité nLPD pour PME suisses de 5 à 25 utilisateurs — sans licence E3/E5.*

Microsoft Purview · Entra ID P1 · Intune + Defender for Business · Copilot Governance — déploiement Minimum Viable de Conformité (MVC) en 4 sessions sur Business Premium + Purview Suite.

Inclut les procédures de déploiement (consultant) et les guides d'exploitation (responsable IT client), avec adaptations sectorielles pour fiduciaires, architectes, avocats, agences de communication et cabinets médicaux.

> *Un socle de conformité nLPD défendable devant le PFPDT, déployable en autonomie sur Business Premium + Purview Suite.*

> ⚠️ *Bundle en cours de rédaction — le guide Purview est publié, les guides Entra ID P1, Intune + Defender et Copilot Governance sont en cours de finalisation.*

---

## 🔐 Sécurité & Durcissement

🆕 **[AiTM / Cookie Hijacking M365 — Détection, mitigation et protection structurelle](https://doit4everyone.github.io/mvc-nlpd-m365/aitm-cookie-hijacking/)**
*Guide technique autonome — Microsoft 365 Business Premium — v1.0 — Août 2026*

Rédigé suite à la divulgation de Mirage2FA (PhaaS AiTM, 20 août 2026) et de CVE-2026-69836 (RCE CVSS 10.0 dans Entra ID, 21 août 2026).

**Partie A — actionnable immédiatement :** CAE, détection des IoC, corrélation SIEM (UTMStack), séquence de réponse à incident, audit rétrospectif post-CVE.

**Partie B — protection structurelle :** Windows Hello for Business par TPM, Cloud Kerberos Trust, AzureADKerberos, CA Authentication Strength (Phishing-resistant MFA), audit des applications legacy, FIDO2 hardware pour comptes à privilèges.

Validé terrain sur infrastructure hybride (Entra Connect + AD on-prem + WS2025) — août 2026.

> *Ce document couvre des nuances rarement documentées : le paradoxe CAE (token de 28h vs révocation temps réel), les restrictions WHfB sur les comptes hybrides privilégiés depuis juin 2026, et la différence réelle entre mitigation et protection structurelle contre AiTM.*

---

## 🔐 Sécurité & SIEM — Lab

**[🛡️ UTMStack Lab v11.2.12 — Guide de déploiement](https://doit4everyone.github.io/utmstack-lab/)** *Déploiement complet UTMStack Community Edition pour PME suisses.*

Installation VMware, intégration Suricata (OPNsense), CrowdSec, dashboards OpenSearch, automatisation SOAR, agents Windows/Linux, Microsoft 365 et Azure.

**En bonus :** Architecture pipeline syslog-ng complète. Règles Suricata custom anti-Mirai. Ban automatique des IPs malveillantes via playbooks SOAR → CrowdSec. Audit NTLM via Windows Event Forwarding en préparation de la migration vers Kerberos (Windows Server 2025). 

**[Pipeline SOC augmenté par IA locale](https://doit4everyone.github.io/utmstack-lab/docs/09-pipeline-llm.html)** (Ollama, n8n) — tri déterministe, comparatif Llama 3.1 / Qwen 2.5 / Mistral Large, retour d'expérience complet sur 12 versions.

**[Intégrations agents et sources de logs](https://doit4everyone.github.io/utmstack-lab/docs/10-integrations-agents.html)** — Agents Windows (5 machines AD) et Linux, Microsoft 365, Azure Event Hub + Event Grid, SOC AI natif.

**[Sysmon v15.21 — Déploiement et configuration](https://doit4everyone.github.io/utmstack-lab/docs/10-sysmon.html)** — Deux configurations XML (postes et DC), méthode registre ANSSI, collecte via Windows Event Forwarding self-subscription locale vers UTMStack.

🆕 **[Règles de corrélation YAML — Chapitre 11](https://doit4everyone.github.io/utmstack-lab/docs/11-correlations-yaml.html)** — 40 règles custom validées en live dans OpenSearch. Séries W (Windows natif), WD (Windows Defender), S (Sysmon via WEF), L (Linux auditd), M (Microsoft 365/Entra ID) et A (Azure Activity Log). 29 techniques MITRE ATT&CK couvertes. Inclut deux règles de détection post-compromission Entra ID (attribution de rôle privilégié, ajout de credentials sur service principal) développées en réponse aux attaques AiTM et à CVE-2026-69836. Les limites du moteur UTMStack v11 sont documentées honnêtement — avec leurs alternatives. **[Bibliothèque de règles YAML sur GitHub](https://github.com/doit4everyone/utmstack-lab/tree/main/rules)**.

> *Un lab opérationnel de détection et réponse aux menaces, avec corrélation Threat Intelligence et enrichissement GeoIP des adresses source — intégrations Microsoft 365 et Azure incluses.*

---

## 🤖 IA locale pour PME suisse

🆕 **[IA locale pour PME suisse — Guide décisionnel 2026](https://doit4everyone.github.io/ia-locale-pme-suisse/)**
*RTX Spark, DGX Spark, RTX PRO 6000, cluster HA, H100 : ce qu'il faut savoir avant d'investir.*

25 pages, sources vérifiées. Architectures disponibles en Suisse, TCO réel sur 3 ans, performances d'inférence mesurées, ingénierie RAG et pipeline de production, sécurité et conformité nLPD.

**Inclus :**
Plan d'apprentissage RAG local — 14 phases, de l'environnement de lab jusqu'aux connecteurs MS 365 et SharePoint Online.
Procédures opérationnelles publiées progressivement au fil de la validation terrain.

> *Rédigé par synthèse de sources publiques vérifiées, sans dépendance à aucun constructeur, revendeur ou intégrateur cité.*

---

## 🧩 Tips & Notes techniques

**[🔓 Tips & Notes techniques — Lab](https://doit4everyone.github.io/tips-lab/)** *Correctifs et retours d'expérience ponctuels, issus de tests en environnement réel.*

Des blocages rencontrés en laboratoire, leurs causes réelles, les solutions qui fonctionnent — sans détour théorique. Rubrique courte, alimentée au fil des découvertes de terrain.

**Premier tip :** [🔓 VMware Workstation bloqué par VBS/UEFI](https://doit4everyone.github.io/tips-lab/docs/01-vmware-vbs-uefi.html) — débloquer la virtualisation imbriquée sur un PC Secured-core récent.

> *Contrairement aux guides complets ci-dessus, ces notes n'ont pas de roadmap : une page, un problème, une solution testée.*

---

## ⚠️ Documentation publiée progressivement

Les guides disponibles sont opérationnels et testés en environnement réel. De nouvelles publications sont ajoutées au fil des travaux de lab et des validations terrain, sans calendrier fixe.

---

## ☕ Soutenir le projet

Ces guides représentent des centaines d'heures de tests en environnements réels, des frais fixes de licences et d'infrastructure.

Si ces ressources vous font gagner du temps, vous pouvez contribuer à l'avancée de mes travaux de lab. Merci.

👉 [![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/R5R31YHNIB)

---

ℹ️ *Références, structuration et aide à la rédaction assistées par IA, avec validation humaine finale.*
