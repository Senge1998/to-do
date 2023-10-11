# to-do
This project deploys the to-do service to kubernetes from a private image repository.

### create secret

To create secret to access the private registry, run the following command and store the imagepullsecrets in the deployment.

`kubectl create secret generic registry-token --from-literal=password-base64=token`

### deploy the manifests to kubernetes

To implement the manifest, what's needed to be done is to run the following command on each manifest

- `kubectl apply -f secrets.yaml`
- `kubectl apply -f service.yaml`
- `kubectl apply -f ingress.yaml`
- `kubectl apply -f deployment.yaml`