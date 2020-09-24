# Deployment #

The scaffolding of this project is built with rules SKAFFOLD (lib google for kubernetes).

The idea is to have a one file skaffold.yaml and this file handle all the .yaml contained in path: infra/k8s/**.yaml.

But for the moment, we will use directly files .yaml

Build image docker with the next command


```bash
cd api
npm run build
```

The next step is tagged the image considering the new version image 

```bash
docker tag auth-quantico us.icr.io/quantico-reader/auth-quantico:1.0.[new version]
```

Push the image

```bash
docker push us.icr.io/quantico-reader/auth-quantico:1.0.[new version]
```


### Environments

The variables environment is contained in kubernetes, you can see with the next command: kubectl get secret.

These variables are mapped in the deploy file, and injected directly into the pod.
