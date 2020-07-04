# deploying-wordpress-kubernetes
----

> To continue make sure you have installed and setup, [cloud SDK](https://cloud.google.com/sdk/install) and [kubectl](https://kubernetes.io/docs/tasks/tools/install-kubectl/).

# deployment
Git clone this repository.
```sh
git clone https://github.com/Manuhmutua/deploying-wordpress-kubernetes.git
```
Then deploy to kubernetes using the kustomization like:
```sh
kubectl apply -k ./
```

# objective
* Create PersistentVolumeClaims and PersistentVolumes
* Create a kustomization.yaml with
    - a Secret generator
    - MySQL resource configs
    - WordPress resource configs
