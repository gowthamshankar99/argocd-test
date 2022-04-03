# argocd-test

## Best Practices around ARGO CD

* ARGO CD gets deployed into the Kubernetes Cluster and creates Custom Resource Definition(Application)
* For multicluster setup, the best practice is to install ARGO in one cluster and have that manage other clusters.
* Updates to different environments of application should use kustomize to replace environment based variables.
* Keep a separate git repo for configuration. ( keep it separate from the App code )
