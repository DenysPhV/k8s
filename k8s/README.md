### dev
`kubectl apply -k k8s/overlays/dev --dry-run=server`

### prod
`kubectl apply -k k8s/overlays/prod --dry-run=server`

### подивитись різницю перед застосуванням
`kubectl diff -k k8s/overlays/dev`


- checking logs
`kubectl logs -n blog-app <pod-name>`  

`echo -n "bloguser" | base64` 

`echo -n "secretpass123" | base64`
