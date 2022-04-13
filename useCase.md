### Capacidades da stack

#### Base dados relacional

O **relational-database-app-kt-plugin** funciona com base no Spring Boot e Spring Data JPA.
Ele adiciona as dependências das bibliotecas necessárias, o driver JDBC referente ao banco de dados escolhido e, caso opte por uma ferramenta de migração, sua dependência também será adicionada.
A configuração básica para utilização do banco de dados relacional é adicionada nos respectivos arquivos do projeto, assim como o código CDK para provisionamento do RDS na AWS.

#### Metrics

O **metrics-app-kt-plugin** é um plugin que tem como objetivo padronizar as métricas geradas pelas aplicações. Ao adicionar o plugin na aplicação é possível escolher se as métricas serão enviadas para o [AWS CloudWatch](https://aws.amazon.com/pt/cloudwatch/) ou para o [Prometheus](https://prometheus.io/docs/introduction/overview/).

#### Tracing

O **tracing-app-kt-plugin** visa padronizar o *tracing* gerado pela aplicação utilizando OpenTelemetry para exportação dos dados.
É possível escolher se o *tracing* gerado será enviado para **Jaeger** ou **AWS X-Ray**.

