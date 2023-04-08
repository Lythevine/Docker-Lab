# DOCKER ARCHITECTURE
**Docker est un ensemble de processus qui tournent sur une machine virtuelle ou pas, il se lance sur le port 2375. La plateforme docker repose sur plusieurs technologies et composants, les principaux sot les suivants:
**Docker Daemon**
Il s'agit d'un processus d'arrière plan persistant qui Il écoute et traite en permanence les requêts d'API docker afin de gerer les images docker, les réseaux, les conteeurs, et les volumes de stockages. 
**Docker client**
C'est la principale interface permettant de communiquer avec le système docker. Il reçoit les commandes par le bias de la  CLI et les transmet au docker daemon.
**Dockerfile**
C'est un fichier texte comportant des instructions de création d'images docker. Il permet de préciser le Système d'exploitation sur lequel sera basée le conteneur, les variables d'environnement, les ports réseaux, les emplacements de fichiers.
**Container** 
Un conteneur est tout simplement l'instance d'une image en cours d'exécution.
**Les images docker**
Il s'agit d'un modèle en leture seule qui contient un ensemble d'instructions pour créer un conteneur pouvant s'exécuter sur la plateforme docker. Les images sont immuables et inchangeables.
**Les volumes docker**
Les volumes dans docker sont des stockages persistants sur la machine haute, mutants et performants qui nous permettent de stocker les données de vos conteneurs. Ils vous permettent de conserver vos données, même en cas de suppression d'un conteneur Docker. Il s'agit également d'une solution pratique pour l'échange de données entre l'hôte et le conteneur.

**Les Endpoint**
Un Endpoint est une extrémité d'un canal de communication.
**Le CLI**
CLI: _Commnand Line Interface_
C'est une interface textuelle qui traite les commandes vers un programme informatique.
Le docker CLI quand à lui est une interface de ligne de commande permettant de communiquer avec le démon de docker.
**Les API**
API: _Application Programming Interface_ 
C'est une interface logicielle qui permet de connecter un logiciel ou un service à un autre logiciel ou service dans le but d'échanger des données et des fonctionnalités.

**Les architectures client serveur**
L’architecture 
Le client: _la commande docker_
Le serveur: _le démon de docker_
Une architecture client-serveur représente l’environnement dans lequel des applications de machines clientes communiquent avec des applications de machines de type serveurs.

Exemple: le navigateur Web d’un client qui demande (on parle de “requête”) le contenu d’une page Web à un serveur Web qui lui renvoie le résultat (on parle de “réponse”).

**Le curl**
Il s'agit d'une interface de ligne de commande qui s'occupe de récupérer le contenu d'une ressource (désignée par une URL) accessible par un réseau informatique.
**La notion de socket sur Linux**
Les sockets sont des points de terminaison mis à l'écoute sur le réseau contenu dans le noyau linux afin d'effectuer les transfers de données. Elles fournissent une interfce qui permet d'utiliser facilement les protocoles de trnsport tels que TCPP et UDP.

**La socket docker**
La socket est utilsée par la Command Line Interface pour exécuter des commandes docker. Le fichier de socket docker est utilisé pour communiquer avec le démon docker c'est aussi le point d'entrée d'API docker. *NB*: Chaque socket tourne sur un port.
Il se situe dans /var/run/docker_sock
**Le réseau dans docker**
Par défaaut lors de l'instllation de docker, il y 3 réseau préconfigurés dont:Le réseau bridge, le réseau none et le réseau host. 
On peut le vérifier avec la commande _docker network ls_
**Le TCP/IP**
TCP:_Transfert Control Protocol_
IP:_Internet Protocol_
Est une suite de protocoles orgnisés en couches utilisés pour le transfert de données sur internet. L'adresse IP permet lors de l'acheminement de données sur le réseau de savoir à chaque embranchement en fonction de cette adresse, quel chemin emprunter.

