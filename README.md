# k8s-lab-gitops

Estado desejado do meu lab de Kubernetes (k3s), aplicado pelo Argo CD.

```
argocd/                 AppProject "lab" + Applications (app-of-apps "lab-root" aponta pra cá)
apps/hello/base/        Deployment, Service e HTTPRoute
apps/hello/envs/dev/    https://hello-dev.k3s.lab:8443  (tag atualizada pelo CI)
apps/hello/envs/prod/   https://hello.k3s.lab:8443      (tag promovida por PR)
```
