### dev
`kubectl apply -k k8s/overlays/dev --dry-run=server`
### prod
`kubectl apply -k k8s/overlays/prod --dry-run=server`

### подивитись різницю перед застосуванням
`kubectl diff -k k8s/overlays/dev`
`kubectl diff -k k8s/overlays/prod`

### Local demostration
`kubectl -n blog-app-dev port-forward svc/blog-app-service 8080:80`

- checking logs
`kubectl logs -n blog-app <pod-name>`  

`echo -n "bloguser" | base64` 

`echo -n "secretpass123" | base64`
