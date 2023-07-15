# Comment run le cluster

- kubectl apply -f postgres-secrets.yaml
- kubectl apply -f postgres-config-map.yaml
- kubectl apply -f persistent-volume.yaml
- kubectl apply -f postgres.yaml
    - kubectl get pods => Attendez que les 3 instances de BDD soit en status "Running"
- kubectl apply -f drupal.yaml
    - kubectl get pods => Pareil pour Drupal

Si avec Minikube,
- minikube service drupal-service

(Théoriquement censé fonctionner ? Je n'arrive pas a accéder au site => "Ce site est inaccessible")