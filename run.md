# Comment run le cluster

Si avec minikube
- minikube addons enable ingress

- kubectl apply -f postgres-secrets.yaml
- kubectl apply -f postgres-config-map.yaml
- kubectl apply -f persistent-volume.yaml
- kubectl apply -f postgres.yaml
- kubectl apply -f drupal.yaml
- kubectl apply -f drupal-ingress.yaml

Si avec Minikube,
- minikube service drupal-service

(Théoriquement censé fonctionner ? Je n'arrive pas a accéder au site => "Ce site est inaccessible")