### Deploy mongodb:

1) kubectl create ns stonehaven-staging (if not done yet)
2) helm repo add authentik https://charts.goauthentik.io (if not done yet)
3) helm upgrade --install authentik authentik/authentik -f values.yml -f values.yml.secret -n stonehaven-staging


### Undo deployment:

1) helm uninstall authentik -n stonehaven-staging