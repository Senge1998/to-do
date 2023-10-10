# to-do

# create secret

To create secret to access the private registry, run the following command and store the imagepullsecrets in the deployment.

kubectl create secret generic registry-token --from-literal=password-base64=cGFzc3dvcmQK

# 