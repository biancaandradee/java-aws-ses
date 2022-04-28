# AMAZON SES (Simple Email Service)
- É um serviço em nuvem de e-mail eficaz, flexível e dimensionável. Com ele, os desenvolvedores podem enviar e-mails de qualquer aplicação. É possível configurar rapidamente a compatibilidade do Amazon SES com vários casos de uso de e-mails, como comunicações transacionais, de marketing ou de e-mails em massa. As opções flexíveis de implantação por IP e autenticação por e-mail do Amazon SES ajudam a aumentar a capacidade de entrega e a proteger a reputação do remetente, enquanto a análise do envio mede o impacto de cada e-mail. 

## Clonando projeto de *torneseumprogramador*
git clone https://github.com/torneseumprogramador/java_aws_sqs_producer_sender.git

# Criando projeto
mvn archetype:generate -DgroupId=br.com.ses_sender -DartifactId=ses_sender -DarchetypeArtifactId=maven-archetype-quickstart -DarchetypeVersion=1.4 -DinteractiveMode=false

# Doc MVN
https://maven.apache.org/guides/getting-started/maven-in-five-minutes.html

### Gerar com manifest
https://www.sohamkamani.com/java/cli-app-with-maven/

# Exemplo de Code Base
https://github.com/awsdocs/aws-doc-sdk-examples/tree/main/javav2

### MVN Options
- mvn validate: validate the project is correct and all necessary information is available
- mvn compile: compile the source code of the project
- mvn test: test the compiled source code using a suitable unit testing framework. These tests should not require the code be - packaged or deployed
- mvn package: take the compiled code and package it in its distributable format, such as a JAR.
- mvn integration-test: process and deploy the package if necessary into an environment where integration tests can be run
- mvn verify: run any checks to verify the package is valid and meets quality criteria
- mvn install: install the package into the local repository, for use as a dependency in other projects locally
- mvn deploy: done in an integration or release environment, copies the final package to the remote repository for sharing with other developers and projects.

## Configurando as variáveis de ambiente
- configurar o .bash_profile ou .bashrc
```shell
code ~/.bash_profile

export AWS_ACCESS_KEY="SUA_ACCESS_KEY"
export AWS_SECRET_KEY="SUA_SECRET_KEY"

source ~/.bash_profile
```

## Rodando o projeto
```shell
./build.sh
./start.sh
```