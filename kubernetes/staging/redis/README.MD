### Deploy mongodb:

1) kubectl create ns stonehaven-staging (if not done yet)
2) helm repo add bitnami https://charts.bitnami.com/bitnami (if not done yet)
3) helm upgrade --install redis bitnami/redis -f kubernetes\staging\redis\values.yml -n stonehaven-staging


### Undo deployment:

1) helm uninstall redis -n stonehaven-staging