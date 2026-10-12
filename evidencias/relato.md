# Relato do grupo

Integrantes: Gharantes
Data: 12/10/2026
Distribuição Linux:
Python 3.14.5 / Docker 29.5.2 / Minikube v1.39.0

## Etapas

| Etapa | Comando e evidência | Resultado esperado | Resultado observado e explicação |
|---|---|---|---|
| Testes | | 8 testes OK | |
| Publicação v1 | | 2 Pods prontos; API v1 | |
| Escala | | 3 Pods prontos | |
| Exclusão e recuperação | | Nome antigo removido; novo Pod criado | |
| ConfigMap | | Mensagem muda após recriar Pods | |
| Atualização v2 | | 3 Pods v2 prontos | |
| Incidente | | Novo Running 0/1; healthz 200, readyz 503 | |
| Rollback | | v2 restaurada | |
| Pipeline v3 | | Smoke OK e estado final v3 | |

## Respostas

1. Por que carregar a imagem no Minikube depois de construir no Docker?
2. Qual a função das portas 8000, 80, 30080 e 8080?
3. Por que o Pod excluído foi substituído?
4. Por que três Pods no mesmo nó não protegem contra a perda da máquina?
5. Por que a mensagem não mudou imediatamente após aplicar o ConfigMap?
6. Tag de imagem e revisão do Deployment são a mesma coisa?
7. Que sinais mostram que a versão quebrada está viva, mas não pronta?
8. O que o timeout fez? O que o rollback restaurou e o que não restaurou?
9. Por que alinhar o arquivo gerado após a reversão?
10. Quais verificações a pipeline realiza? Qual é seu limite?

## Divergências e correções

Descreva hipótese, comando de diagnóstico, sinal observado e correção.
