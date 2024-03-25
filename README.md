# coleta-de-metricas
## 1. tecnologias utilizadas
#### Docker: 
- Utilizado para instalar o prometheus, grafana e jaeger.
- Para rodar, na pasta com o arquivo "docker-compose.yml":
-     docker-compose up
![docker]("docker.png")
#### C# 
- Linguagem utilizada para a escrita do código, na IDE Rider.
#### OpenTelemetry
- É uma biblioteca que serve para coletar e emitir dados de telemetria
- ![pacotes]("pacotes.png")
#### Prometheus
- Utilizado para a coleta das métricas.
Resultado obtido das métricas sem o prometheus:

![resposta]("prometheus.png")
Reaultado obtido para visualização das métricas com o prometheus

  ![prometheus]("prometheus.png")
#### Grafana
- Utilizado para gerar dashboards e alertas com base no prometheus, por exemplo.
- ![grafana]("grafana.png")
#### Jaeger
- Utilizado para mostrar o rastreamento distribuído.
- ![jaeger]("jaeger.png")
## 2. Conceitos aprendidos
### Observabilidade
- É a capacidade de monitorar e analisar a telemetria sobre o estado de cada componente.
- Refere-se à capacidade de entender o comportamento interno de um sistema com base nos dados de entrada e saída, permitindo a detecção, diagnóstico e resolução de problemas.
- É uma combinação de 3 pilares:
    - **logs**: registram operações individuais
    - **métricas**: são contadores de medição e medidores
    - **rastreamento distribuído**: rastreia solicitações e atividades entre componentes em um sistema
      → ajuda a ver onde o tempo é gasto e a rastrear falhas
### Métricas
- Elas são medidas quantitativas que fornecem insights sobre o desempenho e a saúde do sistema. Isso pode incluir métricas como tempo de resposta, taxa de erros e uso de recursos.
- No caso do exemplo desenvolvido, foi desenvolvida uma métrica que acompanha a quantidade de "Greeting" realizados ao longo do tempo.
### Logs
- São registros de eventos ou mensagens geradas pelo sistema durante sua operação.
- São importantes para depuração, monitoramento e auditoria.
- A instrumentação de código pode incluir a captura e o envio de logs para armazenamento e análise, e pode ser feira através do Jaeger
