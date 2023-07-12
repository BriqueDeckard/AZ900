# Compétences mesurées : 

[[_TOC_]]
## Description des concepts de cloud (25 à 30 %) :
### Décrire le cloud computing :
- **Définir le cloud computing :**
> Fournir des services informatiques sur internet : infrastructure informatique (machine virtuelle, stockage, DB, réseau).
> 
> Il n'est pas contraint par l'infra physique.
> Louer la puissance de calcul/le stockage de quelqu'un d'autre.

- **Décrire le modèle de responsabilité partagée :**
> La sécurité physique, l'alimentation electrique, le refroidissement et la connectivité réseau **responsabilité du fournisseur cloud**
> 
> Les données, les accès (sécurité) et les informations **responsabilité du client**

- **Définir les modèles cloud, notamment les modèles publics, privés et hybrides :**
  - **Cloud privé :** Cloud utilisé par une seule entité ( == privé). 
 
    |+|-|
    |-|-|
    |Meilleur contrôle.|Plus de coûts (le materiel doit etre acheté)|
    |Données pas colocalisées| Moins d'avantages (maintenance et mise à jour|
    |securisation élevée||

  - **Cloud public :** Fournisseur de cloud tiers. Tout le monde peut acheter des services cloud, et ensuite accéder aux ressources et les utiliser.
 
    |+|-|
    |-|-|
    |pas de dépense d'investissement (capital) pour scale up |contrôle non total sur les ressources/securité|
    |les app peuvent etre rapidement (dé)provisionnées||
    |on ne paie que ce qu'on utilise||

  - **Cloud hybride :** Utilise à la fois cloud public et cloud privé en interconnection. 
  
    |+|-|
    |-|-|
    |meilleur flexibilité|contrôle la conformité|
    |choix d'où l'application est executée|obligation légales|
    |contrôle la sécurité||
    |contrôle la conformité||
    |||
  **Azure Arc** permet de gérer plus facilement un environnement cloud.

- **Identifier les cas d’usage appropriés pour chaque modèle cloud :**
  - **Cloud privé:** Politiques de sécurité "lourde" ou entreprise soumise a des réglementations complexes.
  - **Cloud hybride:** Reprise après sinistre (datacenter local repose sur du cloud public en cas d'urgence)
  - **Cloud public:** Sauvegarder ses données, se liberer des machines physiques, nouvelles techno

- **Décrire le modèle basé sur la consommation :**
  - **CapEx**: Capital Expenditures : dépenses d'investissement. Dépenses uniques et initiales --> ressources tangibles. (Bâtiment, datacenter ...)
  - **OpEx**: Operationnal Expenditures : services ou produits au fil du temps.
  
  > Cloud computing --> OpEx. On a pas de dépenses "capitales", on ne paye que ce qu'on utilise au fil du temps.

- **Comparer les modèles tarifaires liés au cloud :**
  Paiement a l'utilisation, donc : 
  - Planifier et gerer les cout d'exploit
  - Executer l'infra plus efficacement
  - Adapter la mise à l'échelle aux besoins commerciaux

  > On utilise le centre de données de quelqu'un d'autre, et quand on a fini de s'en servir, on est facturé, et on les rend.

- **Définir le modèle serverless :**
  > laisser le cloud provider fournir, gérer et dimensionner l'infra nécessaire pour faire tourner l'app.

### Décrire les avantages de l’utilisation des services cloud
- **Décrire les avantages de la haute disponibilité et de la scalabilité dans le cloud :**
  - **Haute disponibilité :** Garantir une dispo maximale quels que soient les evenements. Dépend du SLA
  - **Scalabilité :** Ajuster les ressources pour répondre à la demande. Ex: Pic de trafic --> ajouter des ressources
    - **Verticale :** plus de puissance: ajout de processeurs, RAM
    - **Horizontale :** plus de ressources: ajout de VM ou de container.
- **Décrire les avantages de la fiabilité et de la prévisibilité dans le cloud :**
  - **Fiabilité :** capacité d'un système à reprendre son activité apèrs une defaillance. Ex. Ressources déployées sur plusieurs régions du monde. Si catastrophe naturelle, une autre région prend le relai.
  - **Prévisibilité :** Prévisibilité des performances + prévisibilité des couts.
- **Décrire les avantages de la sécurité et de la gouvernance dans le cloud :**
  - **Gouvernance :** les fonctionnalités Cloud permettent de garantir que les ressources déployées sont conformes aux standards d'entreprises et du secteur public. Un audit cloud permet de signaler les ressources non conformes. 
  - **Securité :** IAAS --> controle sur la sécurité maximal, PAAS et SAAS --> patchs et maintenance automatiques
- **Décrire les avantages de la facilité de gestion dans le cloud :**
  > Deux types :
  - **Gestion du cloud :**
    - mise à l'échelle du déploiement des ressources
    - Modèle préconfiguré pour le déploiement
    - Monitoring d'une ou de toutes les ressources
    - Remplacement automatique des ressources defaillantes
    - Alertes automatiques fondées sur des métriques 
  - **Gestion dans les cloud :**
    - Comment on gère environnement et ressources cloud :
      - portail web
      - ligne de commande
      - APIs
      - PowerShell

### Décrire les types de services cloud: 
- **Decrire IaaS :**

  **Definition :**
  > La plus flexible, controle maximal. --> on loue du materiel dans un datacenter cloud.

  **Responsabilités :**
  |Client|Cloud Provider|
  |-|-|
  |installation, configuration et maintenance de l'OS| maintenance du materiel, de la connectivité réseau, de la sécurité physique.|
  |configuration reseau ||
  |configuration DB et stockage ||

  **Cas d'usage :**
  > Migration *lif-and-shift* : ressources dans le cloud similaires à celle du OnPremise, puis transfert des éléments vers le cloud.

- **Decrire PaaS :**

  **Definition :**
  > Compromis entre IaaS et SaaS.

  **Responsabilités :**
  |Client|Cloud Provider|
  |-|-|
  |data, identités, config des app|Infra, sécur physique, connexion a internet, OS, middleware, outils de dev, BI||

  **Cas d'usage :**
  > Utiliser PaaS comme un framework de dev. Permet de développer ou personnaliser des app basées sur le cloud.

- **Decrire SaaS :**

  **Definition :**
  > Le plus complet d'un point de vue produit. On loue une application entièrement développée.

  **Cas d'usage :**
  > Emails, messagerie, Office365 ...