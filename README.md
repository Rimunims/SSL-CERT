Steps to Apply

    Apply the External Service:

kubectl apply -f external-jenkins-service.yaml

Apply the Cert-Manager ClusterIssuer (only if SSL is needed):

kubectl apply -f cert-manager-clusterissuer.yaml

Apply the Ingress:

kubectl apply -f jenkins-ingress.yaml

Verify the Ingress:

    Run:

kubectl get ingress -n new-jenkins3
