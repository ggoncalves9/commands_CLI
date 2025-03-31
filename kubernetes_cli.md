# Criar kubernetes_cli.md
cat <<EOF > kubernetes_cli.md
# KUBERNETES

## Visualizar Recursos
\`\`\`
# Listar pods
kubectl get pods

# Listar serviços
kubectl get svc

# Listar deployments
kubectl get deployments

# Listar PersistentVolumes (PVs)
kubectl get pv

# Listar PersistentVolumeClaims (PVCs)
kubectl get pvc

# Listar Ingresses
kubectl get ingress
\`\`\`

## Descrever Recursos
\`\`\`
# Descrever um pod
kubectl describe pod <pod_name>

# Descrever um serviço
kubectl describe svc <service_name>

# Descrever um PersistentVolume
kubectl describe pv <pv_name>

# Descrever um PersistentVolumeClaim
kubectl describe pvc <pvc_name>
\`\`\`

## Executar Comandos em Pods
\`\`\`
# Executar um comando em um pod
kubectl exec -it <pod_name> -- <command>

# Acessar shell de um pod
kubectl exec -it <pod_name> -- /bin/bash
\`\`\`

## Contextos
\`\`\`
# Listar contextos disponíveis
kubectl config get-contexts

# Trocar de contexto
kubectl config use-context <context_name>

# Visualizar o contexto atual
kubectl config current-context
\`\`\`

## Aplicar Configurações
\`\`\`
# Aplicar um manifesto YAML
kubectl apply -f <file.yaml>

# Excluir recursos definidos em um manifesto YAML
kubectl delete -f <file.yaml>
\`\`\`

## Logs
\`\`\`
# Ver logs de um pod
kubectl logs <pod_name>

# Seguir logs em tempo real
kubectl logs -f <pod_name>
\`\`\`

## Escalar Recursos
\`\`\`
# Escalar um deployment
kubectl scale deployment <deployment_name> --replicas=<number>
\`\`\`

## AWS ELBs (Load Balancers)
\`\`\`
# Listar Load Balancers (ELBs) no AWS
aws elb describe-load-balancers

# Associar um Load Balancer a um serviço Kubernetes
kubectl expose deployment <deployment_name> --type=LoadBalancer --port=<port>
\`\`\`
EOF
