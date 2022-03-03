# Mediastack

Hugo Marques & Emma Durand.
___

# Projet

Création d'une mediastack.

**Outils :**

* radarr : navigateur de recherche qui permet le téléchargement automatique de fichiers (films).
* sonarr : navigateur de recherche qui permet le téléchargement automatique de fichiers (séries).
* plex : lecteur de multimédia pour visionner les séries et films.
* jackett : aggrégateur de torrents et interface pour radarr / sonarr.
* qbittorent : client torrent.

___

**Utilisation**

Sur jackett, il faut configurer les sites de torrent que l'on va utiliser.

Sur radarr et sonarr, il faut configurer nos indexeurs de torrent (jackett) *Torznab* puis spécifier le client qui va télécharger nos films / séries (qbittorrent). Ensuite sur l'interface, via une recherche, on lance le téléchargement automatique du fichier (il apparaît sur qbittorrent).

Une fois le téléchargement terminé, il suffit de se rendre sur plex pour visionner le film ou la série.

___

**Monitoring :**

*Outils :*

* Grafana : outils de supervision pour la visualisation de données.
* Prometheus : base de données.
* qbittorrent-exporter : permet d'exporter les métriques de qbitorrent et de les envoyer dans prometheus.

* stockage ?
* plex ?

___

**Backup**

* Backup

___

**Problèmes rencontrés :**

- permission sur les volumes pour Grafana.
- nom d'hôte des conteuneurs (au lieu du sigle "localhost").

___

# URL

* radarr : http://localhost:7878
* plex : http://localhost:32400/manage
* jackett : http://localhost:9117
* qbittorrent : http://localhost:8080
* sonarr : http://localhost:8989
* qbittorrent-exporter : http://localhost:17871
* prometheus : http://localhost:9090
* grafana : http://localhost:3000
