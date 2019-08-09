# IAD Charts Repository

Questo è un esempio di charts repository.

### Come funziona

E' stata impostata la pagina GitHub alla cartella `docs`. Da lì è possibile pubblicare documenti come questo:

```console
$ helm create mychart
$ helm package mychart
$ mv mychart-0.1.0.tgz docs
$ helm repo index docs --url https://pciaco.github.io/Helm-repo-test/
$ git add -i
$ git commit -av
$ git push origin master
```

Ora è possibile aggiungere il repo `helm repo add Helm-repo-test https://pciaco.github.io/Helm-repo-test/`
