# Strategie de securisation d'une application
![securitee](https://static.vecteezy.com/ti/vecteur-libre/p1/1397516-cyber-securite-illustration-gratuit-vectoriel.jpg)
#### Sommaire

- La compromission des ressources applicatives
- Le vol de donnees
- Denis de services
- XSS
- CSRF
- SQLI
- Defense en profondeur
- Reduction de la surface d'attaque
- Moindre privileges
- Politique de securite des mots de passe
- Securisation de l'authentification 
- Securisation d'API
- HTTPS / TLS / HSTS
- Sanitization
- Journalisation
- SHA256
- Strategie de sauvegarde
- RGPD
- Audit (passi)
- Bug bounty
- SOP
- CORS
- CSP
- SRI
- Clickjacking
- Requetes silencieuses
- Cookies
- Strict mode
- Hashage
- Salage
- authentification vs Autorisation
- RBAC
- 63 recommandations pour le navigateur
- 42 recommandations pour les mots de passe
- Sessions
- Tokens
- API statefull
- API stateless
___

# Quoi ?
La gestion de la sécurité des applications est le processus qui consiste à **développer, ajouter et tester des fonctionnalités de sécurité** au sein des applications, afin **d’éviter les vulnérabilités face à des menaces** telles que les accès et les modifications non autorisés.

# Pourquoi ?
L’expression Sécurité des applications décrit **les mesures de sécurité au niveau des applications** qui aident à **empêcher le vol** ou **le détournement de données** ou de code contenus dans les applications. Elle inclut les considérations portant sur la sécurité qui interviennent lors de la conception et du développement des applications, ainsi que les systèmes et approches de protection des applications après leur déploiement.
___

![suritee2](https://timo.vn/wp-content/uploads/internet-banking-bi-khoa-co-rut-tien-duoc-khong-4.jpg)

> La mis en place d'une startegie de securisation d'une application est une chose tres importante et fait partie des pratiques du developpeur. Les notions de securitees sont diverses et variees, de plus elle ne peuvent et mis en place que si nous comprenont et maitrisont vraiment le sujet.

# La comprimission des ressources applicatives
___
La **compromission des ressources** applicatives est une violation de l’intégrité du contenu, dont une conséquence peut être la défiguration 2 du site. Une telle attaque a pour objectif de modifier
le site pour remplacer le contenu légitime par un contenu choisi par l’attaquant. Il s’agit, par exemple, de relayer un message politique, de dénigrer le propriétaire du site ou simplement de revendiquer l’attaque comme preuve d’un savoir-faire. Une perte d’intégrité peut aussi résulter
en la conduite d’une attaque par point d’eau (watering hole), qui tend un piège aux visiteurs.

# Le vol de donnees
___
Le vol de données est une attaque qui provoque la perte de la confidentialité de certaines données (authentifiants, informations personnelles, informations bancaires, etc.). Elle est réalisée dans un but souvent lucratif et aboutit la plupart du temps à des usurpations d’identité ou à des paiements frauduleux

# Deni de service
___
Le déni de service 3 a pour objet de rendre indisponible le site attaqué pour ses utilisateurs légitimes que ce soit par l’arrêt ou par un ralentissement considérable du service.

# XSS
___
**XSS** : une attaque Cross-Site Scripting (XSS 4) consiste en l’injection de données dans une page
web dans le but de provoquer un comportement particulier du navigateur qui interprète cette
page. Les données injectées ont la forme de langages interprétés par le navigateur tels que
JavaScript ou HTML. Une attaque XSS cible les utilisateurs du site et vise en général à récupérer
des secrets émis ou reçus par ceux-ci (sessions, coordonnées, mots de passe, informations bancaires, etc.), ou bien à effectuer des actions en leur nom.

# CSRF
___
CSRF : Cross-Site Request Forgery (CSRF 5) est une classe d’attaques qui force un utilisateur à exécuter, à son insu, des actions privilégiées sur une application tierce sur laquelle il est authentifié. Ce type d’attaques a lieu lors de la navigation sur un site piégé qui émet des requêtes
vers un site de confiance, mais vulnérable au CSRF

# SQLI
___
SQLi : l’injection SQL (SQLi 7) consiste en la transmission de code malveillant parmi les données entrantes qu’un serveur web utilise pour formuler une requête à destination d’une base de données. Cette classe d’attaques occasionne une perte de contrôle sur les données en base, ce qui peut mener à leur exfiltration, altération ou suppression

# SSRF
___
SSRF : le Server-Side Request Forgery (SSRF 6) est l’équivalent, côté serveur, du CSRF. Il s’agit,
pour un attaquant, de demander au serveur vulnérable d’effectuer des requêtes vers des destinations choisies par l’attaquant en profitant éventuellement des privilèges du serveur (par
exemple, l’accès à un réseau privé) ;

# Defense en profondeur
___
Le principe général de défense en profondeur consiste à mettre en œuvre plusieurs mesures de protection indépendantes en face de chaque menace envisagée.
Il est plus facile d’appliquer ce principe si le système à sécuriser est composé d’unités distinctes, aux interactions bien définies et possédant leurs propres mécanismes de sécurité. La défense en profondeur demande à ce que soient mises en œuvre les mesures de protection nécessaires et disponibles au niveau de chaque unité. Une mauvaise approche est, par exemple, de concentrer toutes les mesures de sécurité au niveau du point d’entrée du système et de constater que les fonctions internes sont complètement exposées en cas de vulnérabilité en amont, ou encore de ne considérer que le risque sur l’infrastructure en ne plaçant comme élément de sécurité qu’un simple pare-feu périmétrique.
Dans l’idéal, chaque brique logicielle de l’application web participe à la protection de l’ensemble du système. L’architecture logicielle du site web ainsi que l’infrastructure d’hébergement doivent participer à la défense en profondeur.

# Reduction de la surface d'attaque
___
La réduction de la surface d’attaque consiste à ne pas exposer des services, accès et autres points
d’entrée s’ils ne sont pas indispensables. Ce principe appliqué au développement logiciel demande que soit limitée la présence de composants logiciels dont l’usage n’est pas strictement nécessaire
au fonctionnement nominal du système, afin de réduire son exposition logicielle. En complément, le système doit également chercher à minimiser son exposition réseau, à la conception comme au déploiement

# Moindre privilleges
___
Ce principe vise à n’octroyer aux éléments et acteurs du système que les permissions strictement nécessaires pour fonctionner, ceci afin de limiter le risque de vol, d’altération ou de destruction de données dans le cas de compromission d’un ou plusieurs éléments.

# Politique de securisation des mots de passe
![password](https://www.protegez-vous.ca/var/protegez_vous/storage/images/7/9/5/4/3254597-1-fre-CA/motes-de-passe.png)

Une politique de sécurité de mots de passe est caractérisée par la définition de certains éléments associés à la gestion des mots de passe (liste non exhaustive) :
- catégorie de mots de passe;
- longueur des mots de passe;
- règles de complexité des mots de passe (c.-à-d. les types de caractères utilisables) ;
- délai d’expiration des mots de passe;
- mécanismes de limitation d’essais d’authentification (cf. la recommandation R10);
- mécanismes de contrôle de la robustesse des mots de passe;
- méthode de conservation des mots de passe;
- méthode de recouvrement d’accès en cas de perte ou de vol des mots de passe;
- mise à disposition d’un coffre-fort de mots de passe.

> Les mots de passe présentent de nombreuses limites à la fois du point de vue de leur utilisation et de leur gestion. Les différentes menaces et attaques connu permettent de catégoriser les mots de passe suivant leurs usages et leur sensibilité à ces attaquants. On peut distinguer trois catégories de mots de passe.
- Les mots de passe devant être mémorisés (sensibles aux attaques en ligne et hors ligne) : concerne
les mots de passe ne pouvant pas facilement être gérés par un coffre-fort de mots de passe, comme le mot de passe maître de ce dernier, le mot de passe d’une session Windows, etc. Ces
mots de passe doivent être mémorisés et suffisamment robustes au vu de leur criticité, mais ils sont peu nombreux à retenir. Cette catégorie de mot de passe étant la plus critique, il est pertinent qu’elle soit associée à un second facteur d’authentification.
- Les mots de passe pouvant ne pas être mémorisés (sensibles aux attaques en ligne et hors ligne) :
concerne les mots de passe pouvant être générés et conservés par des coffres-forts de mots de passe, comme les mots de passe associés à des comptes de récupération.
- Les numéros d’identification personnels, autrement appelés codes PIN sont vérifiés localement au sein d’un composant physique de sécurité. Les codes PIN que l’on retrouve dans les cartes à
puce dont les cartes SIM sont également accompagnés de mesures très restrictives sur le nombre d’échecs d’authentification autorisés (par exemple, la carte se bloque après trois échecs successifs d’authentification).

Cette catégorisation permet de mettre en lumière le fait que parmi tous les mots de passe utilisés
au quotidien, il n’y en a qu’un nombre limité qui doivent être mémorisés par un humain. Cette catégorisation peut alors servir de base pour mener une analyse de risque.
La sécurité des mots de passe est souvent réduite à l’estimation de leur « force », c’est-à-dire l’estimation de leur entropie exprimée en bits. Néanmoins, cette estimation ne vaut que si chaque caractère (respectivement chaque mot) du mot de passe (respectivement de la phrase de passe)
est choisi de manière uniformément aléatoire. Dans le cas contraire, c’est-à-dire dans le cas où les utilisateurs choisissent eux-mêmes leur mot de passe, ils sont habituellement facilement mémorisables comme un mot du dictionnaire, une date, une citation, etc. L’entropie de tels mots de passe se retrouve fortement réduite et son estimation réelle devient très difficile.

# Securisation de l'authentification
___
Pour assurer qu’un utilisateur accède uniquement aux données dont il a besoin, il doit être doté d’un identifiant qui lui est propre et doit s’authentifier avant toute utilisation des moyens informatiques. Les mécanismes permettant de réaliser l’authentification des personnes sont catégorisés selon qu’ils font intervenir :

- ce que l’on sait, par exemple un mot de passe ;
- ce que l’on a, par exemple une carte à puce ;
- une caractéristique propre à la personne, par exemple une empreinte digitale, ou la manière de tracer une signature manuscrite. Pour rappel, la loi Informatique et Libertés subordonne l’utilisation de la biométrie à l’autorisation préalable de la CNIL.

L’authentification d’un utilisateur est qualifiée de forte lorsqu’elle a recours à une combinaison d’au moins deux de ces catégories.
# Les précautions élémentaires
Définir un identifiant unique par utilisateur et interdire les comptes partagés entre plusieurs utilisateurs. Dans le cas où l’utilisation d’identifiants génériques ou partagés est incontournable, exiger une validation de la hiérarchie et mettre en œuvre des moyens pour les tracer.

Respecter la recommandation de la CNIL dans le cas d’une authentification des utilisateurs basée sur des mots de passe, notamment en stockant les mots de passe de façon sécurisée et en appliquant les règles de complexité suivantes pour le mot de passe :

- au moins 8 caractères comportant 3 des 4 types de caractères (majuscules, minuscules, chiffres, caractères spéciaux) si l’authentification prévoit une restriction de l’accès au compte (cas le plus courant) comme :
- une temporisation d’accès au compte après plusieurs échecs ;
- un « Captcha » ;
- un verrouillage du compte après 10 échecs ;
- 12 caractères minimum et 4 types de caractères si l’authentification repose uniquement sur un mot de passe
Et encore bien d'autre choses...

#### Menace et attaques sur l'authentification
La principale menace contre laquelle l’authentification cherche à se protéger est l’usurpation d’identité, qui consiste pour un attaquant à se faire passer pour un utilisateur légitime auprès du vérifieur.
Il est possible de distinguer deux grands types d’attaquants.

**Attaquant en ligne** : l’attaquant peut uniquement interagir avec le serveur d’authentification
pour tenter de retrouver une valeur secrète (un mot de passe ou une clé privée par exemple).
Il doit par exemple être capable d’interagir avec un serveur Web afin de réaliser son attaque.
Se protéger contre des attaquants en ligne nécessite de mettre en place des mesures spécifiques,
comme le blocage temporaire de l’accès au compte pendant plusieurs secondes, voire minutes,
après un certain nombre d’essais infructueux (cf. recommandation R10).
**Attaquant hors ligne** : l’attaquant peut interagir avec le serveur d’authentification, et a également accès aux données permettant au vérifieur de contrôler l’identité du prouveur (par
exemple des empreintes de mots de passe ou une clé publique). L’attaquant n’a pas besoin d’interagir avec le serveur pour réaliser son attaque et a alors accès à une puissance de calcul potentiellement très importante.

#### De nombreux types d’attaques peuvent être menés contre un protocole d’authentification
- les attaques par force brute : tests automatisés de tous les mots de passe et de toutes les clés
cryptographiques possibles;
- les attaques sur le protocole d’authentification : attaques de l’homme-du-milieu, attaques par
rejeu, exploitation de vulnérabilité de l’implémentation, etc. (voir section 2.5 pour plus de détails);
- le vol du moyen d’authentification : vol d’une carte à puce, récupération d’un mot de passe par
hameçonnage, manipulation par l’ingénierie sociale, etc.

> Pour contrer ces menaces il est evident que l'utilisateur doit se prevenir de tous ces desagrements en prenant de bonnes pratiques. Cette bonne pratique est de choisir des mots de passe dits robustes ils doivent être suffisamment longs, suffisamment complexes (avec l’utilisation de minuscules, majuscules, chiffres et caractères spéciaux).

# Recommandations concernant le cycle de vie des facteurs d'authentification
![recommendations](https://cdni.iconscout.com/illustration/premium/thumb/cyber-security-2974902-2477419.png)
### Le cycle de vie d’un facteur d’authentification peut se décomposer en trois phases :
- sa creation
- son utilisation
- sa revocation

#### Pour limitee l'impact d'une usurpation d'identitee de nombreuses recommandations et mecanismes existe.

Les phases de création et d’enregistrement d’un facteur d’authentification sont des étapes primordiales et critiques pour toute authentification. Un attaquant qui parviendrait à récupérer ou modifier des informations d’authentification lors de l’enregistrement, ou bien encore des éléments
cryptographiques qui ne seraient pas générés correctement (voir par exemple le retrait de certains
facteurs matériels d’authentification présentant un défaut de générateur aléatoire [35]) sont autant
de vecteurs d’attaque qui peuvent alors compromettre le reste de l’authentification.

# Securisation d'API
![api](https://i3.wp.com/venturebeat.com/wp-content/uploads/2022/10/GettyImages-API_APIs_API-security_1317706831-e1665416483886.jpg?resize=780,470)

# HTTPS / TLS / HSTS
___
La mise en place de HTTPS a pour objectif :
- de garantir, autant que possible, l’authenticité du site consulté ;
- de garantir également l’intégrité et la confidentialité des données échangées en bloquant les attaques de type Man-In-The-Middle (écoute, interception ou modification des échanges à la volée par des tiers, à l’insu de l’utilisateur).

Une attaque de type Man-In-The-Middle expose les utilisateurs du site web à l’injection de contenu malveillant pouvant conduire, entre autres, à la consultation de pages piégées incitant au
téléchargement de codes malveillants ou à des attaques par rebond, que cela soit sur le réseau local de la victime, ou sur des sites tiers sur lesquels la victime a un compte. Ce type d’attaque cible
des utilisateurs légitimes d’un site accessible en clair, et ne dépend pas de son contenu. Notamment, ces attaques peuvent toucher les utilisateurs d’un site dynamique comme statique.

> La mise en place de HTTPS doit cependant respecter les bonnes pratiques en vigueur. À ce jour, les versions préconisées pour la mise en œuvre d’HTTPS sont TLSv1.2 et TLSv1.3

# R1 - Mettre en œuvre TLS à l'état de l'art
Il est nécessaire de mettre en œuvre les Recommandations de sécurité relatives à TLS pour tout site même si celui-ci ne traite pas d’informations sensibles.
Pour éviter de perdre du trafic, les sites web acceptent souvent des connexions en HTTP et les redirigent vers HTTPS, laissant ainsi à un attaquant l’opportunité d’intercepter cette communication. L’utilisation de HTTP Strict Transport Security (HSTS, [7]) indique au navigateur d’utiliser
automatiquement HTTPS pour tous les accès au site web. Il empêche également un utilisateur d’accepter de poursuivre la navigation sur un site non sécurisé en outrepassant les alertes de sécurité
(certificat invalide, certificat généré par une autorité non reconnue, etc.) levées par les navigateurs.
# R2 - Mettre en œuvre HSTS
Il est nécessaire de mettre en œuvre HSTS afin de limiter les risques d’attaque de type Man-In-The-Middle dus à des accès non sécurisés générés par les utilisateurs ou par un attaquant.
> Attention ! - Attention, la pérennité de l’accès en HTTPS est un prérequis indispensable à HSTS, qui rendra l’accès en clair impossible.

Le mise en œuvre de HSTS se fait par la transmission d’un en-tête HTTP lors de l’accès au site
en HTTPS pour assurer son intégrité. Par défaut, la stratégie HSTS d’un site est enregistrée par le
navigateur lorsqu’il est visité pour la première fois (trust on first use). Pour combler cette vulnérabilité initiale, le gérant d’un site peut décider de l’inscrire à une « liste préchargée » (voir HSTS preload 10) de sites accessibles seulement en HTTPS, connue à l’avance par les navigateurs.

# Sanitization
![sanitization](https://www.iscot.it/wp-content/uploads/2020/03/Overview_22_1065x438.png)

# Journalisation
___
Les journaux d’événements constituent une brique technique indispensable à la gestion de la sécurité des systèmes d’information. L’activité de journalisation est un moyen de détection des incidents
de sécurité et d’analyse du comportement d’un site ou d’une application web. Cette activité concerne la phase de conception de l’application, pour la génération de journaux (ex. traçabiltié d’un changement de privilèges), ainsi que la phase d’exploitation de l’application, pour laquelle l’application des Recommandations de sécurité pour la mise en œuvre d’un système de journalisation est nécessaire. En effet, les recommandations portant sur l’horodatage des événements ainsi que sur
la synchronisation des horloges entre les composants sont particulièrement pertinentes dans le cas d’une application web, bien souvent décomposée en plusieurs services amenés à générer leurs propres journaux de façon isolée. Il faudra donc parvenir à les corréler pour analyser et comprendre les événements de sécurité remontés par un outil prévu à cet effet. De plus, l’exposition élevée
d’une application web fait des journaux d’événements et d’erreurs des moyens exploitables par un attaquant dans le but de réaliser des attaques de déni de service par saturation des journaux, ou encore pour exfiltrer les données sensibles parfois incluses dans certains journaux d’erreur. Il convient
donc, malgré le caractère indispensable d’un système de journalisation, de respecter les bonnes pratiques visant à éviter que son utilisation puisse être détournée ou ses données corrompues lors
d’une attaque

# SHA256
![sha](https://academy.bit2me.com/wp-content/uploads/2018/07/18_Sha256-1.png)

# Strategie de sauvegarde
![save](https://globbsecurity.fr/wp-content/uploads/2018/09/sauvegarde-702x336.jpg)

# RGPD
___
# Audit (passi)
___
Les bonnes pratiques de conception évoquées jusqu’ici doivent s’accompagner de processus permettant de détecter les vulnérabilités du site web. La mise en œuvre de ces processus se décline sous la forme d’actions manuelles et automatisées, lors des phases de conception comme d’exploitation de l’application web. Côté automatisation, on peut citer l’ajout de modules d’analyse à la chaîne d’intégration continue (ex. : détection de dépendances vulnérables, outils d’analyses

# Bug bounty
![bb](https://mpost.io/wp-content/uploads/Bug-Bounty.jpg)

# SOP
![sop](https://static.vecteezy.com/system/resources/previews/002/265/691/original/sop-standard-operating-procedure-concept-design-vector.jpg)

# CORS
___
Il est parfois nécessaire de contourner la SOP (stratégie de sécurité par défaut du navigateur) afin de permettre l’appel de ressources en dehors de l’Origin telles que peuvent en fournir des services web tiers de météo ou d’actualités par exemple. La méthode utilisée dans ce cas est nommée CrossOrigin Resource Sharing. Cette méthode est normalisée et vient en remplacement de plusieurs autres techniques jusqu’alors utilisées mais considérées comme dangereuses et limitées telles que la proxyfication ou l’utilisation de JSON with Padding (JSON-P).
**CORS** est un standard qui permet la définition explicite d’un contrat entre le serveur web et le
navigateur qui spécifie les conditions d’acceptation d’échanges Cross-Origin. La négociation de ce
contrat a lieu par l’intermédiaire d’en-têtes HTTP selon la cinématique suivante :
1. une requête Cross-Origin présente au serveur destinataire l’en-tête Origin fixé par le navigateur
avec l’adresse du site en cours de consultation ;
2. le serveur précise dans l’en-tête de réponse Access-Control-Allow-Origin l’adresse du site
depuis laquelle il accepte de répondre.
Cette réponse peut être explicite Access-Control-Allow-Origin: %ORIGINE_ADMISE% ou implicite Access-Control-Allow-Origin: * ;
3. le navigateur reçoit la réponse et analyse l’en-tête Access-Control-Allow-Origin.
Dans le cas général, si celui-ci est * ou égal à l’Origin courante, la réponse est acceptée. Dans
le cas contraire la réponse est bloquée et une exception de sécurité est levée par le navigateur.

# CSP
___
Content Security Policy (CSP) permet de définir une stratégie de contrôle des accès aux ressources atteignables d’un site web donné par l’application de restrictions sous forme de liste d’autorisations (aussi appelée liste blanche).
La maîtrise de l’ensemble des ressources récupérées par un site web permet de réduire le risque d’apparition et l’exploitabilité de vulnérabilités XSS, la définition de la liste des ressources autorisées peut être effectuée en utilisant :
- l’en-tête HTTP dédié, Content-Security-Policy, dans la réponse HTTP ;
- la balise équivalente, <meta http-equiv="Content-Security-Policy">, dans la réponse HTML.

# SRI
___
# Clickjacking
___
Le détournement de clic, ou clickjacking, est un type d’attaque dans lequel une page web trompeuse incite un utilisateur légitime à cliquer sur du contenu en apparence légitime qui le mène en réalité à effectuer des actions, à son insu, sur d’autres sites. Ces attaques sont en général mises en œuvre au moyen d’une page piégée incluant des cadres (iframes) invisibles qui pointent vers des sites légitimes sur lesquels l’utilisateur piégé a ouvert une session

# Requetes silencieuse
___
Certaines fonctionnalités de la spécification HTML permettent de demander au navigateur d’émettre des requêtes silencieuses sans passer par l’exécution de code JavaScript ou CSS. Comme tout comportement qui conduit le navigateur d’une victime à initier une connexion de manière silencieuse, ces requêtes sont potentiellement indésirables et présentent des risques allant de la
fuite d’informations jusqu’à l’exploitation de failles CSRF en passant par la réalisation d’attaques par déni de service distribué (DDoS).
Un premier exemple de ce genre de fonctionnalités est l’attribut ping. Une balise HTML (a) peut, si celle-ci présente un attribut href, comporter un attribut ping en complément. L’attribut ping contient alors une liste d’URLs vers lesquelles seront réalisées des requêtes POST lorsque le lien
sera cliqué. Les URLs définies par l’attribut ping peuvent se situer en dehors de l’Origin et son utilisation relève généralement du tracking publicitaire.
L’attribut ping est implémenté par le navigateur et ne met pas en jeu l’utilisation de JavaScript pour émettre des requêtes silencieuses. Sa mise en œuvre augmente donc le risque CSRF, parce que les contre-mesures qui visent à interdire la transmission d’un cookie de session lors d’une requête issue d’un script ne s’appliquent pas. Par ailleurs, ping permet de démultiplier efficacement le nombre de requêtes émises lors du clic sur un lien, et de piéger des victimes afin de distribuer une attaque par déni de service, puisque la cible du lien peut être légitime sans que la présence ou la
valeur de l’attribut ping soit visible par un utilisateur non spécialiste.

# Cookies
___
Cookie : l’accès à un cookie suit une stratégie similaire mais légèrement différente de SOP.Notamment, le chemin qui suit le nom de domaine est contrôlé, mais le port n’est pas pris en compte. En outre, un même cookie peut être envoyé sur plusieurs sous-domaines différents.

# strict mode
___
Le mode strict 22 de JavaScript permet de désactiver certains comportements jugés trop souples lors de l’interprétation, dans des domaines tels que la syntaxe ou encore les types. Une fois le mode strict activé, toute erreur ignorée dans le mode par défaut sera considérée comme une exception et interrompra le fil d’exécution JavaScript. Le mode strict oblige le développeur
JavaScript à plus de rigueur et désactive également les fonctionnalités en voie d’obsolescence, dont l’implémentation n’est valable qu’au titre de la rétrocompatibilité. Il peut être conservé en phase de production afin de contrarier une tentative d’injection de code JavaScript (vulnérabilité XSS).
Ce mode se déclare au niveau d’un fichier ou au niveau d’une fonction par l’ajout de la chaîne de caractères "use strict"; 23. Dans les deux cas, cette chaîne de caractères doit être la première directive rencontrée. Attention, dans le cas de la déclaration au niveau du fichier, l’utilisation d’outils
de minification de code peut rendre la directive globale à tous les fichiers. Au contraire, si les outils de génération de code ne positionnent pas "use strict"; au début du fichier généré mais après d’autres instructions, la directive sera ignorée pour l’ensemble du fichier.

> Il est recommandé de déclarer l’utilisation du mode strict en utilisant la directive "use strict"; au début de chaque fonction JavaScript. Pour couvrir l’ensemble du code, l’utilisation de fonctions auto-invoquées est préférable à la mise en œuvre du mode strict au niveau du fichier.

# Hashage 
![hash](https://www.blockchains-expert.com/wp-content/uploads/2017/11/Algorythm-de-hachage.jpg)

# Salage
___
Utiliser un sel aléatoire long. Il est recommandé d’utiliser un sel choisi aléatoirement pour chaque compte et d’une longueur d’au moins 128 bits.
Les fonctions de hachage cryptographique recommandées, comme la famille SHA2, sont des fonctions très rapides à exécuter, ce qui, dans le contexte du stockage des mots de passe, est un avantage pour les attaquants, leur permettant de tester (c.-à-d. de calculer des empreintes) de nombreux
mots de passe. Afin de ralentir les attaquants, il est recommandé d’utiliser des fonctions de dérivation de mots de passe dites memory-hard permettant à la fois d’augmenter le temps d’exécution
mais aussi l’espace mémoire lors du calcul d’une empreinte. L’utilisation de telles fonctions correctement paramétrées permet un important ralentissement des attaques par force brute tout en
ayant un impact négligeable sur les services légitimes ne devant exécuter qu’un petit nombre de calculs d’empreintes. En particulier les fonctions de dérivation de mots de passe memory-hard permettent de se protéger contre des attaquants profitant des accélérations matérielles apportées par
l’utilisation de cartes graphiques ou de hardware dédié.

# Authentification vs Autorisation
___
L’authentification est un mécanisme faisant intervenir deux entités distinctes : un **prouveur** et
**vérifieur**
**Le prouveur** cherche à prouver son identité au vérifieur. Il s’agit par exemple pour le prouveur
de démontrer sa connaissance d’une donnée secrète comme un mot de passe.
**Le vérifieur** doit être capable de s’assurer de la validité de l’identité du prouveur. Il s’agit par
exemple pour le vérifieur de contrôler l’exactitude du mot de passe fourni par le prouveur

Un prouveur est un utilisateur du système d’information cherchant à s’authentifier. Le vérifieur est
quant à lui classiquement un serveur du système d’information qui a la charge de vérifier l’identité
d’un utilisateur.
Une premierer etape est necessaire avant de proceder a l'authentification, il faut tout d'abord que l'utilisateur renseigne les informations le concernant.
- son identitee
- son moyen d'authentification

et encore bien d'autre chose ...
Cette etape est **l'enregistrement**, elle consiste a enregistrer un prouveur aupres d'un verifieur.

**L’authentification** est précédée par une phase **d’identification** (parfois implicite) qui consiste, pour
le prouveur, à annoncer son identité sans prouver cette dernière. La fonction d’authentification en tant que telle a pour objectif de permettre au prouveur de démontrer son identité. Une fois l’authentification réalisée, cette dernière (ou un autre service) va permettre d’autoriser
l’accès d’un utilisateur a des ressources (donnees, services, applications, ect...).

# RBAC
![rbac](https://assets.website-files.com/5ff66329429d880392f6cba2/60a2467ccc346830c07f2325_RBAC%20preview.jpg)

# 63 recommandations pour le navigateur
___
# 42 recommadations pour les mots de passe
___

![recommandation2](https://www.p1technology.com.au/uploads/117/90/10-steps-cyber-security.jpg)
# R1 - Privilégier l'authentification multifacteur
Il est recommandé de privilégier l’utilisation d’une authentification multifacteur,
c’est-à-dire une authentification mettant en œuvre plusieurs facteurs d’authentification appartenant à une catégorie de facteur différente parmi les facteurs de connaissance, de possession et inhérent.

# R2 - Privilégier l'utilisation de moyens d'authentification forts
Il est recommandé de privilégier l’utilisation de moyens d’authentification forts reposant sur des mécanismes cryptographiques conformes au RGS et à ses annexes
# R3 - Conduire une analyse de risque
Il est recommandé de mener une analyse de risque pour déterminer les moyens d’authentification à mettre en œuvre en fonction du besoin de sécurité

# R4 - Créer les facteurs d'authentification dans un environnement maîtrisé
Il est recommandé de créer les facteurs d’authentification dans un environnement
maîtrisé par l’entité chargée de sa création. Les méthodes d’enregistrement et de remise du facteur d’authentification doivent être cohérentes avec le niveau de sécurité attendue de l’authentification
# R5 - Générer les éléments aléatoires avec un générateur de nombres aléatoires
robuste
Il est recommandé de générer les éléments aléatoires nécessaires à l’authentification (comme des clés cryptographiques par exemple) au moyen d’un générateur de
nombres aléatoires robuste conforme à l’annexe B1 du RGS [13].

# R6 - Remettre les facteurs d'authentification au travers de canaux sécurisés
Dans le cas où le facteur d’authentification est remis à l’utilisateur (cas d’une carte à puce par exemple), il est recommandé de privilégier la remise en main propre car elle rend possible la vérification d’identité présentant le meilleur niveau d’assurance. Dans le cas d’une remise à distance, il est recommandé que les canaux et moyens de transmission utilisés pour délivrer le facteur d’authentification soient protégés en intégrité, authenticité et confidentialité. La vérification de l’identité à distance est également possible et est réglementée par le référentiel d’exigences applicables aux prestataires de vérification d’identité à distance (PVID).

# R7 - Mettre en place un processus de renouvellement des facteurs d'authentification
Il est recommandé de mettre en place un processus de renouvellement des facteurs d’authentification
 # R8 - Ne pas utiliser le SMS comme moyen de réception d'un facteur d'authentification
Il est recommandé de ne pas utiliser le SMS comme moyen de réception d’un facteur d’authentification.
# R8 - Ne pas utiliser le SMS comme moyen de réception d'un facteur d'authentification
Il est recommandé de ne pas utiliser le SMS comme moyen de réception d’un facteur
d’authentification.

# R9 - Conserver les historiques d'utilisation des facteurs d'authentification
Il est recommandé de conserver les historiques des évènements liés à la vie des facteurs d’authentification afin de faciliter la détection de comportements anormaux
qui présagerait d’une compromission d’un facteur d’authentification. Parmi ces évènements, on peut citer : la date de création, les tentatives d’authentification (réussiesou échouées), les demandes de renouvellement, la date de révocation, etc. Il est recommandé de suivre le guide de recommandations de sécurité pour la mise en œuvre
d’un système de journalisation [6] appliqué au contexte de l’authentification.

# R10 - Limiter dans le temps le nombre de tentatives d'authentification
Il est recommandé de mettre en œuvre un mécanisme limitant le nombre de tentatives d’authentification sur une période de temps donnée, afin de réduire les probabilités d’authentifications frauduleuses par force brute.

# R11 - Réaliser l'authentification au travers d'un canal sécurisé
Il est recommandé de réaliser l’authentification au travers d’un canal sécurisé
(comme un flux encapsulé par les protocoles TLS ou IPsec) permettant de garantir
des propriétés de confidentialité, d’intégrité et d’authenticité.

# R12 - Limiter la durée de validité d'une session authentifiée
Il est recommandé qu’une session authentifiée ait une durée maximale de validité. Les secrets temporaires de sessions (comme des cookies par exemple) doivent avoir une durée de vie limitée. Il est ainsi recommandé de forcer la ré-authentification des
utilisateurs après une période adaptée au cas d’usage. Des recommandations concernant la bonne gestion d’une session authentifiée (en
particulier concernant les cookies) peuvent être trouvées dans le guide Recommandations pour la mise en oeuvre d’un site Web : maîtriser les standards de sécurité côté
navigateur.

# R13 - Protéger les données d'authentification stockées par le vérifieur
Lorsque des données d’authentification doivent être conservées par le vérifieur, il est recommandé d’assurer la protection en confidentialité et en intégrité de ces informations. Il est également recommandé de protéger les accès à ces données sensibles.

# R14 - Ne pas donner d'information sur l'échec de l'authentification
Il est recommandé que l’échec d’une authentification multifacteur ne donne pas d’information sur le facteur ayant conduit à l’échec de l’authentification.

# R15 - Définir un délai d'expiration des facteurs d'authentification
Il est recommandé de mettre en place un délai d’expiration des facteurs d’authentification, permettant de limiter une éventuelle période d’utilisation frauduleuse

# R16 - Définir une politique d'utilisation des facteurs d'authentification
Il est recommandé d’établir une politique définissant les conditions d’utilisation du ou des facteurs d’authentification mis en place. Il peut par exemple s’agir de définir les conditions d’utilisation d’un facteur d’authentification de possession, de définir les procédures qu’un utilisateur doit suivre dans les cas de perte ou de compromission
de son facteur d’authentification.

# R17 - Sensibiliser les utilisateurs à la sécurité de l'authentification
Il est recommandé de mettre en place des campagnes de sensibilisation des utilisateurs aux risques liés à l’authentification (par exemple des campagnes de sensibilisation au hameçonnage). Les utilisateurs doivent être également informés des différentes conditions d’utilisation des facteurs d’authentification mis à leur disposition.

# R18 - Mettre en place un processus de révocation des facteurs d'authentification
Il est recommandé de mettre en place un processus dédié permettant de révoquer
des facteurs d’authentification et de diffuser l’information de révocation.

# R19 - Définir des délais adaptés de prise en compte des révocations
Les délais pour la prise en compte et l’application de la révocation doivent faire partie de l’analyse de risque et doivent être adaptés aux menaces pesant sur le système d’information.

# R20 - Mettre en place une politique de sécurité des mots de passe
Il est recommandé de mettre en place une politique de sécurité des mots passe adaptée au contexte et aux objectifs de sécurité du système d’information.

# R21 - Imposer une longueur minimale pour les mots de passe
Il est recommandé de définir une longueur minimale pour les mots de passe lors de leur création en fonction du niveau de sécurité visé par le système d’information.

# R22 - Ne pas imposer de longueur maximale pour les mots de passe
Selon les systèmes, il est recommandé de ne pas fixer de limite à la longueur maximale d’un mot de passe afin de permettre aux utilisateurs d’avoir recours à des phrases de passe ou longs mots de passe.

# R23 - Mettre en œuvre des règles sur la complexité des mots de passe
Au moment de la création ou du renouvellement d’un mot de passe par un utilisateur, il est recommandé de mettre en œuvre des règles de complexité tout en proposant un jeu de caractères le plus large possible.

# R24 - Ne pas imposer par défaut de délai d'expiration sur les mots de passe des comptes non sensibles
Si la politique de mots de passe exige des mots de passe robustes et que les systèmes permettent son implémentation, alors il est recommandé de ne pas imposer par défaut de délai d’expiration sur les mots de passe des comptes non sensibles comme les comptes utilisateur.

# R25 - Imposer un délai d'expiration sur les mots de passe des comptes à privilèges
Il est recommandé d’imposer un délai d’expiration sur les mots de passe des comptes très sensibles comme les comptes administrateurs. Ce délai d’expiration peut par exemple être fixé à une durée comprise entre 1 et 3 ans.

# R26 - Révoquer immédiatement les mots de passe en cas de compromission suspectée ou avérée
En cas de compromission suspectée ou avérée d’un système d’authentification, tous les mots de passe concernés par ce système doivent être renouvelés immédiatement (de l’ordre de la journée). Au-delà de ce délai, les comptes concernés doivent être désactivés et une procédure de réactivation pour les utilisateurs doit être mise en œuvre.

# R27 - Mettre en place un contrôle de la robustesse des mots de passe lors de leur
création ou de leur renouvellement Il est recommandé de procéder à un contrôle automatisé et systématique de la robustesse des mots de passe au moment de leur création ou de leur renouvellement.

# R28 - Utiliser un sel aléatoire long
Il est recommandé d’utiliser un sel choisi aléatoirement pour chaque compte et d’une longueur d’au moins 128 bits.

# R29 - Utiliser une fonction de dérivation de mots de passe memory-hard pour
conserver les mots de passe Pour conserver les mots de passe, il est recommandé d’utiliser des fonctions de dérivation de mots de passe memory-hard comme scrypt ou Argon2.
Il est conseillé de paramétrer ces fonctions de manière à proposer le niveau de
sécurité le plus élevé possible tant que cela n’affecte pas un usage légitime.

# R30 - Proposer une méthode de recouvrement d'accès
Afin de permettre aux utilisateurs de retrouver un accès à leur compte, il est recommandé de mettre en place une méthode de recouvrement d’accès adaptée au
contexte d’utilisation.

# R31 - Mettre à disposition un coffre-fort de mots de passe
Il est recommandé que les responsables du système d’information mettent à disposition des utilisateurs un coffre-fort de mots de passe et les forment à son utilisation.

# R32 - [Utilisateur] Utiliser des mots de passe robustes
Il est recommandé d’utiliser des mots de passe (ou phrases de passe) robustes, c’està-dire suffisamment longs et complexes pour résister aux attaques par recherche exhaustive et n’étant pas un mot du dictionnaire (ou une citation ou phrase connue) pour résister aux attaques par dictionnaire.

# R33 - [Utilisateur] Utiliser un mot de passe différent pour chaque service
Il est recommandé d’utiliser un mot de passe différent pour chaque service auquel l’utilisateur est inscrit.

# R34 - [Utilisateur] Utiliser un coffre-fort de mots de passe
Il est recommandé d’utiliser un coffre-fort de mots de passe permettant facilement de générer des mots de passe robustes et différents pour chaque service, facilitant la mise en œuvre de la recommandation R33.

# R35 - [Utilisateur] Protéger ses mots de passe
Il est recommandé d’adopter les bons réflexes de protection des mots de passe. Par exemple, il est impératif de ne pas écrire ses mots de passe sur une note sous le clavier, de ne pas créer un fichier « mot de passe » sur le poste utilisateur, de ne pas s’envoyer ses mots de passe par courriel, etc. L’utilisation d’outils comme les coffresforts de mots de passe est à privilégier.

# R36 - [Utilisateur] Utiliser un mot de passe robuste pour l'accès à sa messagerie électronique
Il est recommandé d’utiliser un mot de passe robuste pour accéder à sa messagerie électronique. En particulier, il faut privilégier l’utilisation d’une méthode d’authentification multifacteur lorsque cela est disponible.

# R37 - [Utilisateur] Choisir un mot de passe sans information personnelle
Il est recommandé de ne pas construire son mot de passe à partir d’informations
personnelles comme les noms et prénoms ou encore la date de naissance.

# R38 - [Utilisateur] Modifier les mots de passe par défaut
Il est recommandé de modifier les mots de passe par défaut.

# R39 - Utiliser un facteur de possession intégrant un composant de sécurité qualifié ou certifié
Il est recommandé de recourir à l’utilisation d’un facteur de possession dont le composant de sécurité a reçu un visa de sécurité de l’ANSSI.

# R39- - Utiliser un facteur de possession intégrant un composant de sécurité
Lorsqu’une authentification, simple facteur ou multifacteur, utilise un moyen d’authentification reposant sur un facteur de possession, il est recommandé qu’il possède un composant de sécurité intégré.
Il est recommandé d’utiliser un protocole d’authentification conforme au RGS.

# R39-- - Utiliser un facteur de possession même sans composant de sécurité
L’utilisation d’un facteur de possession permet l’utilisation de protocoles d’authentification conformes au RGS. Son utilisation reste recommandée même si les éléments secrets ne peuvent pas être stockés dans un composant de sécurité. Dans ce contexte, il est essentiel de mettre en œuvre des mesures de protection supplémentaires comme le chiffrement des éléments cryptographiques, des restrictions d’accès,
etc.
# R40 - Ne pas utiliser un facteur inhérent comme unique facteur d'authentification
Il est recommandé de ne pas utiliser un facteur d’authentification inhérent lorsqu’il s’agit d’une authentification avec un unique facteur.

# R41 - Utiliser un facteur inhérent uniquement associé à un facteur d'authentification fort
Dans le cadre d’une authentification multifacteur, si un facteur d’authentifcation inhérent est utilisé, alors il est recommandé de l’accompagner d’au moins un autre facteur d’authentification reposant sur un mécanisme cryptographique conforme au RGS.

# R42 - Favoriser une rencontre en présence lors de l'enregistrement d'un facteur
inhérent Lors de la phase d’enregistrement d’un moyen d’authentification inhérent, il est recommandé de procéder à la vérification de l’identité par une rencontre en présence afin de limiter les risques d’usurpation d’identité lors de cette phase.

# Sessions
![session](https://www.vevox.com/getmedia/a46979ef-7ae7-431f-b37d-ab4caf32a42e/Artboard-1-copy-3.png)

# Tokens
![token](https://i0.wp.com/blockchainfrance.net/wp-content/uploads/2018/05/token.png?fit=1331%2C698&ssl=1)

# API statefull
![fullvsless](https://www.interviewbit.com/blog/wp-content/uploads/2021/12/Stateful-Vs-Stateless.png)
#  API stateless
