k3d cluster create k3d-cluster-989 --servers 3 --agents 2 --k3s-arg "--disable=servicelb@server:*"

k3d cluster delete k3d-cluster-989

helm repo add metallb https://metallb.github.io/metallb


helm repo add bitnami https://charts.bitnami.com/bitnami

helm install my-release bitnami/wordpress