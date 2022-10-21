    Replace authentication details, database details and DNS details in config.yaml file. 

    Add Jupypter HUB chart repository 

$ helm repo add jupyterhub https://jupyterhub.github.io/helm-chart/ 
$ helm repo update 
 

To Install the helm chart  with below command: 

$ helm upgrade --cleanup-on-fail --install jupyterhub jupyterhub/jupyterhub --namespace mi-v3-5 --values config.yaml

To uninstall:
helm uninstall jupyterhub --namespace mdh-cpv-dev
