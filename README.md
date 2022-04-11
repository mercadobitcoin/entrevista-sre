# entrevista-sre

Neste lab, você deverá: 

1. Acessar o console do Google Cloud Platform e subir um cluster de Kubernetes: \
Obs: Você tem liberdade para criar via Console GCP ou usar ferramentas para IAC, como por ex. Terraform.
- Detalhes e especificações:
  - Projeto GCP id: (Você receberá o id do projeto e o horário de liberação do acesso)
  - Criar um Cluster Kubernetes (GKE Standard mode)
  - Número de nodes: 3
  - Location: Qualquer região US
  - Control plane: Configs default
2. Instalar o Helm chart [hello-kubernetes](https://github.com/mercadobitcoin/entrevista-sre/tree/main/k8s/helm/hello-kubernetes) usando a tag v.1.10 da imagem
3. Garantir que o(s) pod(s) esteja com status Running, configurado para o mínimo de 4 instâncias no autoscaling.
4. Garantir que o deployment tenha liveness e readiness no /
5. O tipo de Service deve ser compatível com o nome do workload
6. Suba um cronjob que imprima seu nome a cada 5 minutos
7. Fazer algumas requisições para o IP público do LoadBalancer
8. Acessar o IP Público do LoadBalancer pelo seu Browser e salvar um printscreen da tela. Clique no link que aparecer no browser.
9. Pegar algumas linhas de log do pod, referente a requisição acima.
10. Reunir todos os arquivos gerados (logs, imagens, scripts) e entregue da forma que achar melhor.

Documente suas decisões e explique suas soluções. 