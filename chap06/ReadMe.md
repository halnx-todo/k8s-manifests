# Remarques

Dans ces manifests, nous utilisons minikube. Les images sont builder avec le docker de minikube `eval $(minikube docker-env)`.
Pour cela l'attribut `pod.spec.containers[]?.imagePullPolicy` est mis a `IfNotPresent`. minikube etant local, vous ne puller pas les images depuis un depots d'image docker.

