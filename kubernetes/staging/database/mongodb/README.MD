### Deploy mongodb:

1) kubectl create ns stonehaven-staging (if not done yet)
2) helm repo add bitnami https://charts.bitnami.com/bitnami (if not done yet)
3) helm upgrade --install mongodb bitnami/mongodb -f kubernetes\staging\database\mongodb\values.yml --set "auth.rootUser=XXX,auth.rootPassword=XXX" -n stonehaven-staging


### Undo deployment:

1) helm uninstall mongodb -n stonehaven-staging