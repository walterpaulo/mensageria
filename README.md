# Mensageria

Producer -> Manda mensagens, api ...

<p>
Consumer -> recebe mensagens, serviço de email ...


## RabbitMQ

```
$ docker run -d --hostname my-rabbit --name some-rabbit -p 8080:15672 rabbitmq:3-management
```
> usuário e senha guest


## Kafka

* kafka 3.1.0
* Gradle 7.4.1
* Java 11

Baixe o código fonte [fonte](https://dlcdn.apache.org/kafka/3.1.0/kafka-3.1.0-src.tgz)

```
wget https://dlcdn.apache.org/kafka/3.1.0/kafka-3.1.0-src.tgz

```

Extrai arquivo
```
tar xf kafka-3.1.0-src.tgz -C ~/

cd kafka-3.1.0-src/

./gradlew jar

echo "alias "start_zookeeper=\'sh ~/kafka-3.1.0-src/bin/zookeeper-server-start.sh ~/kafka-3.1.0-src/config/zookeeper.properties\'" 
alias "start_kafka=\'sh ~/kafka-3.1.0-src/bin/kafka-server-start.sh ~/kafka-3.1.0-src/config/server.properties\'"" >> ~/.bashrc

source ~/.bashrc

```
*tempo de 20 minutos para rodar *gradle jar

### Pacote
* default-jdk
* gradle**

#### **Gradle

```
sudo mkdir /opt/gradle && cd /opt/gradle
sudo wget https://services.gradle.org/distributions/gradle-7.4.1-bin.zip
sudo unzip gradle-7.4.1-bin.zip
echo "export PATH=$PATH:/opt/gradle/gradle-7.4.1/bin" >> ~/.bashrc
source ~/.bashrc
```

