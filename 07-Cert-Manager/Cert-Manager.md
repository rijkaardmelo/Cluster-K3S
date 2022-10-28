<h1 align = "center"> Instalação e Configuração Cert-Manager </h1>

<h2 align = "center"> Na máquina do administrador do Cluster </h2>

<h2> Instalando Cert-Manager </h2>

1 - Adicionando Cert-Manager no repositório Helm

    helm repo add jetstack https://charts.jetstack.io

2 - Atualizando o repositório Helm

    helm repo update

3 - Instalando Cert-Manager

    helm install cert-manager jetstack/cert-manager --namespace cert-manager --create-namespace --set installCRDs=true