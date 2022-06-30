# Create kubernetes secret from with the gitlab access token
kubectl create secret generic gitlab-credentials -n crossplane-system --from-literal=gitlab-credentials="<ACCESS_TOKEN>"

# We can create the gitlab token from the Gitlab web UI or CLI

# Only install the provider YAML for Helm and k8s Crossplane Provider. The ProviderConfig will be created automatically for the remote cluster in the next step when the k8s cluster is created.