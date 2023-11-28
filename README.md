# kubernetes-demo

  
## Ambiente de desenvolvimento

Para o ambiente de desenvolvimento, utilizaremos o minikube para nos comunicarmos com a API do Kubernetes.


1. Inicie um cluster com 3 nodes para testes utilizando o seguinte comando:

``` bash
minikube start --nodes 3
```

2. Inicie o dashboard do minikube:

``` bash
minikube dashboard
```

Obs: a utilização de ferramentas como dashboard pode apresentar problemas de segurança, pois o usuário tem permissões administrativas ao cluster. É possível monitorar o cluster a partir do terminal, os comandos mais utilizados são:

- `kubectl get pods` para listar todos os pods disponíveis no cluster e seus estados.
- `kubectl logs` seguido do nome do Pod para ver seus logs.
- `kubectl get svc` para listar todos os serviços disponíveis no cluster e seus parâmetros.
- `kubectl get cj` para listar todos os agendamentos.
- `kubectl api-resources` para mostrar tudo o que está disponível no cluster.
- `kubectl describe` seguido de um recurso como `pods` ou `svc` para ter uma descrição completa do recurso, podendo ser seguido por um único nome de recurso focando a descrição em apenas um alvo.