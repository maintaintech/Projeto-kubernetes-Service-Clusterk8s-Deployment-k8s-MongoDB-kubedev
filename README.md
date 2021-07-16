# Projeto-kubernetes-Service-Clusterk8s-Deployment-k8s-MongoDB-kubedev


#### Utilizando; Linux/K3d/K8s/Vscode/dockerHub


- 1*Criação do dockerfile da image da aplicação com os arquivos node.js
dockerfile

- 2*Criação do arquivo de manifesto do cluster kubernetes, utilizando o banco de dados MongoDB
deployment.yaml

- 3*Criação do arquivo do Service/MongoDB/ClusterIP
service.yaml

- 4*Criando o arquivo de API do cluster com a image que foi criada no dockerfile e feito o docker push msilvaops/api-produto

- 5*Após subir a aplicação e realizar o deployment vamos acrescentar 10 replicas ou seja 10 cluster que seria os containers os pods
atualizando e adicionando na linha 6 do codigo replicas: 10
aplicando e reconfigurando o arquivo com kubectl apply -f  ./ caminho do arquivo.
deployment.yaml

#### Conclusão; Facilidade de gerenciamento com uma boa performance ao trabalhar na construção com 3 elementos do Kubernetes que são;

- 1:Pod; fica a baixo executando os containers

- 2:Replicaset; fica como controlador gerenciando a escalabilidade e a resiliencia do pod através do gerenciamento de replicas em contaners.

- 3:Deployment; fica acima do Replicaset  gerenciando a troca de versão da aplicação realizando atualização da aplicação no deployment

#### O loadbalancer expondo o pod externo para poder acessar.

# Com isso podemos alterar e atualizar aplicação em tempo real em down time 0.

# A solução com deploy eficiente no kubernetes com esses 3 elementos.

Referencia do projeto KubeDev criador da aplicação API-Cadastro de Produtos Node.js
