# monitoring
Tout d'abord j'ai suivi tout les commandes de l'installer de Prometheus avec Helm , kube-state-metrics et le monitoring du cluster et les étapes pour le déployement de notre application d’exemple (goprom) et la connection à prometheus. Voici les captures suivante:

L'interface de service goprom

![text](1.png)

L'interface de service goprom-metrics

![text](2.png)

et aprés pour tester le service prometheus-server j'ai changer le type en mode NodePort par l'application grphique Lens :

![text](3.png)

Puis j'ai vérifiée que prometheus récupère bien les métriques de l’application avec la requête PromQL :

![text](4.png)

Et derniérement étape j'ai installer et configurer Grafana pour visualiser les requêtes :

Connection a grafana :   

![text](5.png)

L'ajout de DataSource : 

![text](6.png)

La creation de dashboard :

![text](7.png)

et finalement la visualisation du graph :

![text](8.png)