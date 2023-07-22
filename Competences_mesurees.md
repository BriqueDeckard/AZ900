# Compétences mesurées : 

## Description des concepts de cloud (25 à 30 %)
- Décrire le cloud computing
  - Définir le cloud computing
  - Décrire le modèle de responsabilité partagée
  - Définir les modèles cloud, notamment les modèles publics, privés et hybrides
  - Identifier les cas d’usage appropriés pour chaque modèle cloud
  - Décrire le modèle basé sur la consommation
  - Comparer les modèles tarifaires liés au cloud
  - Définir le modèle serverless

- Décrire les avantages de l’utilisation des services cloud
  - Décrire les avantages de la haute disponibilité et de la scalabilité dans le cloud
  - Décrire les avantages de la fiabilité et de la prévisibilité dans le cloud
  - Décrire les avantages de la sécurité et de la gouvernance dans le cloud
  - Décrire les avantages de la facilité de gestion dans le cloud
  
- Décrire les types de services cloud
  - Décrire IaaS (infrastructure as a service)
  - Décrire PaaS (platform as a service)
  - Décrire SaaS (software as a service)
  - Identifier les cas d’usage appropriés pour chaque service cloud (IaaS, PaaS et SaaS)

## Décrire l’architecture et les services Azure (35 à 40 %)
- Décrire les principaux composants architecturaux d’Azure
  - Décrire les régions, les paires de régions et les régions souveraines Azure
  - Décrire les zones de disponibilité
  - Décrire les centres de données Azure
  - Décrire les ressources et les groupes de ressources Azure
  - Décrire les abonnements
  - Décrire les groupes d’administration
  - Décrire la hiérarchie des groupes de ressources, des abonnements et des groupes d’administration

- Décrire les services de calcul et réseau Azure
  - Comparer les types de calcul, notamment les conteneurs, les machines virtuelles et les fonctions
  - Décrire les options de machine virtuelle, notamment les machines virtuelles Azure, Azure Virtual
  Machine Scale Sets, les groupes à haute disponibilité et Azure Virtual Desktop
  - Décrire les ressources nécessaires aux machines virtuelles
  - Décrire les options d’hébergement d’applications, notamment les applications web, les conteneurs
  et les machines virtuelles
  - Décrire le réseau virtuel, notamment l’objectif des réseaux virtuels Azure, des sous-réseaux
  virtuels Azure, de l’appairage, d’Azure DNS, de la passerelle VPN Azure et d’ExpressRoute
  - Définir des points de terminaison publics et privés

- Décrire les services de stockage Azure
  - Comparer les services de stockage Azure
  - Décrire les différents niveaux de stockage disponibles dans Azure
  - Expliquer les options de redondance disponibles pour assurer la résilience des données
  - Identifier les options de compte de stockage et les types de stockage disponibles
  - Utiliser les options de déplacement de fichiers, telles que AzCopy, Explorateur Stockage Azure 
  et Azure File Sync
  - Décrire les options de migration, notamment Azure Migrate et Azure Data Box

- Décrire l’identité, l’accès et la sécurité Azure
  - Décrire les services d’annuaire dans Azure, notamment Azure Active Directory (Azure AD), 
  solution Microsoft Entra, et Azure Active Directory Domain Services (Azure AD DS)
  - Décrire les méthodes d’authentification dans Azure, notamment l’authentification unique 
  (SSO), multifacteur (MFA) et sans mot de passe
  - Décrire les identités externes dans Azure, notamment le B2B (entreprise-entreprise) 
  et le B2C (entreprise-client)
  - Décrire l’accès conditionnel dans Azure AD
  - Décrire le contrôle d’accès en fonction du rôle (RBAC)
  - Décrire le concept de Confiance Zéro
  - Décrire l’objectif du modèle de défense en profondeur
  - Décrire l’objectif de Microsoft Defender pour le cloud

## Décrire la gestion et la gouvernance Azure (30 à 35 %)
- Décrire la gestion des coûts dans Azure
  - Décrire les facteurs qui peuvent affecter les coûts dans Azure
  - Comparer la calculatrice de prix et la calculatrice du coût total de possession (TCO)
  - Décrire les fonctionnalités de gestion des coûts dans Azure
  - Décrire l’objectif des étiquettes
- Décrire les fonctionnalités et les outils dans Azure pour la gouvernance et la conformité
  - Décrire l’objectif de Microsoft Purview dans Azure
  - Décrire la finalité d’Azure Policy
  - Décrire la finalité des verrous de ressources
- Décrire les fonctionnalités et outils de gestion et de déploiement des ressources Azure
  - Décrire le portail Azure
  - Décrire Azure Cloud Shell, notamment l’interface de ligne de commande Azure (CLI) et Azure PowerShell
  - Décrire l’objectif d’Azure Arc
  - Décrire l’infrastructure en tant que code (IaC)
  - Décrire Azure Resource Manager (ARM) et les modèles ARM
- Décrire les outils de monitoring dans Azure
  - Décrire l’objectif d’Azure Advisor
  - Décrire Azure Service Health
  - Décrire Azure Monitor, notamment Log Analytics, les alertes Azure Monitor et Application Insights


## Description des concepts de cloud (25 à 30 %) :
### Décrire le cloud computing :
- **Définir le cloud computing :**
> Fournir des services informatiques sur internet : infrastructure informatique 
(machine virtuelle, stockage, DB, réseau).
> 
> Il n'est pas contraint par l'infra physique.
> Louer la puissance de calcul/le stockage de quelqu'un d'autre.

- **Décrire le modèle de responsabilité partagée :**
> La sécurité physique, l'alimentation electrique, le refroidissement et la 
connectivité réseau **responsabilité du fournisseur cloud**
> 
> Les données, les accès (sécurité) et les informations **responsabilité du client**

- **Définir les modèles cloud, notamment les modèles publics, privés et hybrides :**
  - **Cloud privé :** Cloud utilisé par une seule entité ( == privé). 
 
    |+|-|
    |-|-|
    |Meilleur contrôle.|Plus de coûts (le materiel doit etre acheté)|
    |Données pas colocalisées| Moins d'avantages (maintenance et mise à jour|
    |securisation élevée||

  - **Cloud public :** Fournisseur de cloud tiers. Tout le monde peut acheter des services cloud, 
  et ensuite accéder aux ressources et les utiliser.
 
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
  - **CapEx**: Capital Expenditures : dépenses d'investissement. Dépenses uniques et initiales 
  --> ressources tangibles. (Bâtiment, datacenter ...)
  - **OpEx**: Operationnal Expenditures : services ou produits au fil du temps.
  
  > Cloud computing --> OpEx. On a pas de dépenses "capitales", on ne paye que ce qu'on utilise au fil du temps.

- **Comparer les modèles tarifaires liés au cloud :**
  Paiement a l'utilisation, donc : 
  - Planifier et gerer les cout d'exploit. Ex: Je vais avoir besoin de tant de VM, sur tant de 
  temps, combien cela peut e couter ?
  - Executer l'infra plus efficacement.
  - Adapter la mise à l'échelle aux besoins commerciaux. Ex: Nouvelle fonctionnalité plus
  consommatrice de ressource : je prévoie de déployer en conséquences

  > On utilise le centre de données de quelqu'un d'autre, et quand on a fini de s'en servir, 
  on est facturé, et on les rend.

- **Définir le modèle serverless :**
  > laisser le cloud provider fournir, gérer et dimensionner l'infra nécessaire pour faire tourner l'app.

### Décrire les avantages de l’utilisation des services cloud
- **Décrire les avantages de la haute disponibilité et de la scalabilité dans le cloud :**
  - **Haute disponibilité :** Garantir une dispo maximale quels que soient les evenements. 
  Dépend du SLA. Ex: La demande User augmente, alors on scale pour répondre sans interruptions.
  - **Scalabilité :** Ajuster les ressources pour répondre à la demande. 
  Ex: Pic de trafic --> ajouter des ressources
    - **Verticale :** plus de puissance. Ex: ajout de processeurs, RAM
    - **Horizontale :** plus de ressources. Ex: ajout de VM ou de container.
- **Décrire les avantages de la fiabilité et de la prévisibilité dans le cloud :**
  - **Fiabilité :** capacité d'un système à reprendre son activité apèrs une defaillance. 
  Ex. Ressources déployées sur plusieurs régions du monde. Si catastrophe naturelle, une autre région prend le relai.
  - **Prévisibilité :** Prévisibilité des performances + prévisibilité des couts.
- **Décrire les avantages de la sécurité et de la gouvernance dans le cloud :**
  - **Gouvernance :** les fonctionnalités Cloud permettent de garantir que les ressources déployées
  sont conformes aux standards d'entreprises et du secteur public. Un audit cloud permet de signaler
  les ressources non conformes. Ex: Azure Advisor qui donne des recommandations sur la fiabilité, la sécurité, etc
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
  |installation, configuration et maintenance de l'OS| maintenance du materiel, de la 
  connectivité réseau, de la sécurité physique.|
  |configuration reseau ||
  |configuration DB et stockage ||

  **Cas d'usage :**
  > Migration *lif-and-shift* : ressources dans le cloud similaires à celle du OnPremise, puis 
  transfert des éléments vers le cloud.

- **Decrire PaaS :**

  **Definition :**
  > Compromis entre IaaS et SaaS.

  **Responsabilités :**
  |Client|Cloud Provider|
  |-|-|
  |data, identités, config des app|Infra, sécur physique, connexion a internet, OS, middleware, outils de dev, BI||

  **Cas d'usage :**
  > Utiliser PaaS comme un framework de dev. Permet de développer ou personnaliser des
  app basées sur le cloud.

- **Decrire SaaS :**

  **Definition :**
  > Le plus complet d'un point de vue produit. On loue une application entièrement développée.

  **Cas d'usage :**
  > Emails, messagerie, Office365 ...

## Décrire l’architecture et les services Azure (35 à 40 %)
### Décrire les principaux composants architecturaux d’Azure
- **Décrire les régions, les paires de régions et les régions souveraines Azure**
  - **Géography:**
  Une zone du globe qui contient une ou plusieurs régions. Elle préserve la résidence des données
  et garantie certaines limites de conformité. Ex: India, USA or UK
  - **Région:**
  Une zone géo qui contient au moins un centre de données. Ils sont relié entre eux ar des réseaux
  à faible latence. Ex: East USA, North USA
  - **Paire de région:**
  une association de deux régions spécifiques au tarvers d'une geographie dans le but d'assurer des
  fonctionnalités de reprise après sinistre avancées.
  - **Région souveraine:**
  Une region dédiée à une entité "souveraine" comme les Azure Government : Gouvernement US,
  Azure Chine. Ces régions sont isolées du reste d'Azure.

- **Décrire les zones de disponibilité**

  Des centres de données physiquements séparés dans une région. Ils sont prévus comme une limite 
  d'isolation :  si l'une tombe en panne, une autre prend le rela. Elles sont connectés par des 
  réseau de fibre optique privée très rapide.
  
- **Data Center:**
  
  Le bâtiment qui habrite les racks de serveurs. C'est la brique physique élémentaire de 
  l'infrastructure materielle Azure.

- **Décrire les ressources et les groupes de ressources Azure**

  - **Ressource**
  Le bloc élémentaire de la gestion Azure. Tout ce qu'on crée/déploie/provisionne sur Azure est une ressource.

  - **Groupe de ressource**
  Regroupement logique de ressources. Lorsqu'on crée une ressource, elle doit etre placée dans un
  groupe de ressource. Une action sur l groupe se répercute sur toutes les ressources qu'il contient. 

- **Décrire les abonnements**

  Une brique qui permet de faciliter la gestion, la facturation et la mise à l'échelle. 
  Comme les groupes de ressources regroupent les ressources, les abonnements regroupent les groupes
  de ressources et facilitent la facturation. 
  **Utiliser Azure necessite de posséder au  moins UN abonnement. **
  Avec les abonnements, on peut appliquer a la fois des stratégies de gestion d'accès et des modèles 
  de facturation. Les abo permettent également de définir des limites autour des produits. 
  - **Limites autour du produit:**
  Il existe deux types de limites a appliquer autour du produit Azure : 
    - **Les limites de facturation:**
    Définie la façon dont l'utilisation du Cloud Azure est facturée à un compte Azure. Ainsi on peut
	créer plusieurs abonnements en fonction des conditions de facturation désirées : Azure va générer
	des factures et des rapports de facturation distincts pour chaque abonnement. 
    - **Les limites de contrôle d'accès:**
    Azure permet d'appliquer des stratégies de gestion des accès au niveau de l'abonnement. Cela 
	permet de créer des abonnements distincts en fonction des structures organisationnelles.

- **Décrire les groupes d’administration**

  Quand on a plusieurs abonnements, le groupe d'administration est une unité logique qui permet 
  d'organiser les abonnements et de les gérer plus facilement (accès, stratégie, conformité). 
  C'est le bloc qui permet de gérer "à grande échelle".


- **Décrire la hiérarchie des groupes de ressources, des abonnements et des groupes d’administration**

  Comme les groupes d'administration peuvent etre imbriqués, on peut s'en servir pout appliquer des
  stratégies et une gestion des accès unifiés.
  Ex : 
  > Un groupe d'A racine
  >
  >> Un groupe d'A "RH"
  >>
  >>> Abonnement RH-1
  >>>
  >>> Abonnement RH-Test
  >>>
  >> Un groupe d'A "SI"
  >>
  >>> Abonnement SI-Dev
  >>>
  >>> Abonnement SI-PreProd
  >>>

  Ex: Si on applique une stratégie de sécurité au groupe d'A racine, alors cette politique de 
  sécurité va s'appliquer sur toutes les ressources de tous les abonnements.

  Ex: En créant une RBAC dans le groupe d'A SI, j'autorise (selon mes conditions) mes utilisateurs 
  à accéder à la fois aux ressources de l'abonnement de Dev et celui de Preprod.

  **A noter que :** 
  - 10 000 groupes d’administration peuvent être pris en charge dans un seul annuaire.
  - Une arborescence de groupes d’administration peut prendre en charge jusqu’à six niveaux de 
  profondeur. Cette limite n’inclut pas le niveau Racine ni le niveau de l’abonnement
  - Chaque groupe d’administration et chaque abonnement ne peut avoir qu’un seul parent

### Décrire les services de calcul et réseau Azure
- **Comparer les types de calcul, notamment les conteneurs, les machines virtuelles et les fonctions**
  - **Conteneurs**
  Permette de réondre au problème Une VM == un OS, puisqu'on peut exceuter plusieurs instances de 
  conteneur sur une même machine. Conçu pour etre géré dynamiquement. Souvent utilisé avec une
  architecture en micro-services. Ex. on a un conteneur DB, un contenur backend, un coneneur front. 
  Selon les besoins, on peut doubler une instance de l'un ou de l'autre pour scaler facilement.
  
  - **Machines virtuelles**
  Infrastructure IaaS. Serveur virtualisé. Permet d'eviter d'avoir a acheter et entretenir du
  materiel, mais necessite installer/configurer/mettre à jour les logiciels qui s'executent dessus.
  Un choix idéal quand on doit : 
    - Avoir le contrôle de l'OS
	- Executer des logiciels personnalisés.
	- Config d'herbergement personnalisé

  - **Fonctions**
  Service de calcul Serverless, piloté par des events. Ne demande pas de maintenance. Avec une VM, 
  la ressource doit etre déployé pour que le service puisse fonctionné. Avec une Function, c'est un
  évènement qui va venir déclencher la fonction. 
  Quand il n'y a pas d'appel, on ne fai rien, on ne paye pas. Se met à l'échelle automatiquement. 
  
- **Décrire les options de machine virtuelle, notamment les machines virtuelles Azure, Azure Virtual Machine Scale Sets, les groupes à haute disponibilité et Azure Virtual Desktop**

  - **VM Azure**
  - **Azure VM Scale Sets**
	Groupes de VM identiquesà charge équilibrée. Permet de gérer, configurer et mettre à jour un 
	grand nombre de machines virtuelles de manière centralisée. Déploie automatiquement un équilibreur
  de charge.
  - **Groupe a haute disponibilité**
  Echelonne les mise à jour. 
    - **Domaine de mise à jour:**
	VM qui peuvent etre redémarrées en même temps lors d'une mise à jour == un seul groupe "HS" à 
	la fois. 30 mn avant le demarrage du groupe suivant.
	- **Domaine d'erreur:**
	Regroupe les VM selon une alimentation et un commutateurs réseau commun. Si un grupe tombre, les autres groupes restent.
	
  - **Azure Virtual Desktop**
  Un service de virtualisation des postes de travail. Permet, par exemple, d'executer un poste de travail windows depuis n'importe quel endroit.
  
- **Décrire les ressources nécessaires aux machines virtuelles**
- **Décrire les options d’hébergement d’applications, notamment les applications web, les conteneurs et les machines virtuelles**
  - **Applications web**
  - **Conteneurs**

  - **VM**
- **Décrire le réseau virtuel, notamment l’objectif des réseaux virtuels Azure, des sous-réseaux virtuels Azure, de l’appairage, d’Azure DNS, de la passerelle VPN Azure et d’ExpressRoute**
  - **Reseau vituel**
  - **Sous réseau**
  - **Peering**
  - **Azure DNS**
  - **Passerelle VPN Azure**
  - **Express Route**
- **Définir des points de terminaison publics et privés**
  - **Point de terminaison public**
  - **Point de terminaison privé**