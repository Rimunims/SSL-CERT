##Steps to Apply

##Apply the External Service:

    kubectl apply -f external-jenkins-service.yaml

Apply the Cert-Manager ClusterIssuer (only if SSL is needed):

    kubectl apply -f cert-manager-clusterissuer.yaml

Apply the Ingress:

    kubectl apply -f jenkins-ingress.yaml

Verify the Ingress:

Run:

    kubectl get ingress -n new-jenkins3

``bash
kubectl create secret generic jenkins-auth-secret --from-literal=auth="your-username:your-api-token" -n new-jenkins3
``
