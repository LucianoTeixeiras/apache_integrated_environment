# apache_integrated_environment
Este repositório foi criado para fornecer um ambiente de desenvolvimento completo e integrado para estudo e prática com tecnologias modernas de processamento de dados, armazenamento, orquestração de pipelines e análise de dados. O objetivo principal é facilitar a experimentação e o aprendizado prático com ferramentas amplamente utilizadas no ecossistema de Big Data e Data Engineering.

This repository was created to provide a complete and integrated development environment for studying and practicing modern technologies for data processing, storage, pipeline orchestration, and data analysis. The primary goal is to facilitate experimentation and hands-on learning with widely used tools in the Big Data and Data Engineering ecosystem.

# Apache Integrated Environment

Este projeto configura um ambiente de desenvolvimento integrado utilizando Docker para estudo e prática de diversos componentes essenciais no ecossistema de dados.

## Componentes e Objetivos Principais

- **Apache Spark**: Framework de processamento distribuído para Big Data.
- **Apache Kafka**: Plataforma de streaming de eventos para construção de pipelines de dados em tempo real.
- **Apache Zeppelin**: Ferramenta para criação de notebooks interativos integrados com Spark.
- **MinIO**: Serviço de armazenamento compatível com S3.
- **Apache Airflow**: Orquestrador de workflows e pipelines de dados.
- **Metabase**: Ferramenta de visualização e análise de dados.
- **Scala**: Linguagem funcional e orientada a objetos, amplamente utilizada com Spark.
- **R**: Ambiente para computação estatística e gráficos.
- **Python**: Linguagem de programação versátil para ciência de dados, desenvolvimento de aplicações e scripts.

## Estrutura do Projeto

```
docker-dev-env/
├── docker-compose.yml
├── Dockerfiles/
│   ├── spark/
│   │   └── Dockerfile
│   ├── kafka/
│   │   └── Dockerfile
│   ├── zeppelin/
│   │   └── Dockerfile
│   ├── airflow/
│   │   └── Dockerfile
│   ├── metabase/
│   │   └── Dockerfile
│   ├── minio/
│   │   └── Dockerfile
```

## Configuração do Ambiente

### Pré-requisitos

- Docker
- Docker Compose
- Conta no GitHub configurada com chave SSH ou autenticação HTTPS

### Passos para Configuração

1. **Clone ou Crie o Repositório**

   Crie um diretório local:
   ```bash
   mkdir apache_integrated_environment
   cd apache_integrated_environment
   ```

2. **Inicialize o Repositório Git**
   ```bash
   git init
   git branch -M main
   ```

3. **Adicione os Arquivos do Projeto**
   Insira os arquivos do projeto ou copie-os para o diretório criado.

4. **Realize o Commit Inicial**
   ```bash
   git add .
   git commit -m "Initial commit for Apache Integrated Environment"
   ```

5. **Crie o Repositório no GitHub**
   Acesse sua conta do GitHub e crie um repositório chamado `apache_integrated_environment`.

6. **Adicione o Repositório Remoto**
   Substitua `LucianoTeixeiras` pelo seu nome de usuário do GitHub:
   ```bash
   git remote add origin https://github.com/LucianoTeixeiras/apache_integrated_environment.git
   ```

7. **Envie os Arquivos para o GitHub**
   ```bash
   git push -u origin main
   ```

### Iniciando o Ambiente

1. **Construa os Contêineres**
   ```bash
   docker-compose build
   ```

2. **Inicie os Contêineres**
   ```bash
   docker-compose up -d
   ```

3. **Acesse os Serviços**
   - Spark Master: [http://localhost:8080](http://localhost:8080)
   - Zeppelin: [http://localhost:8081](http://localhost:8081)
   - Airflow: [http://localhost:8082](http://localhost:8082)
   - Metabase: [http://localhost:3000](http://localhost:3000)
   - MinIO: [http://localhost:9000](http://localhost:9000)
   - Kafka Broker: `localhost:9092`
   - Zookeeper: `localhost:2181`

### Finalizando o Ambiente

Para parar e remover os contêineres:
```bash
docker-compose down
```

Para remover volumes e redes associados:
```bash
docker-compose down -v
```

---

## Contribuindo

Contribuições são bem-vindas! Abra um pull request ou issue no repositório GitHub.

---

## Licença

Este projeto é disponibilizado sob a [MIT License](LICENSE).
