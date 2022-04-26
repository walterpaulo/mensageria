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

* versão 3.1.0

Baixe o código fonte [fonte](https://dlcdn.apache.org/kafka/3.1.0/kafka-3.1.0-src.tgz)

```
wget https://dlcdn.apache.org/kafka/3.1.0/kafka-3.1.0-src.tgz

cd kafka-3.1.0-src/
```

Extrai arquivo
```
tar xf kafka-3.1.0-src.tgz -C ~/

echo "alias "start_zookeeper=\'sh ~/kafka-3.1.0-src/bin/zookeeper-server-start.sh ~/kafka-3.1.0-src/config/zookeeper.properties\'" 
alias "start_kafka=\'sh ~/kafka-3.1.0-src/bin/kafka-server-start.sh ~/kafka-3.1.0-src/config/server.properties\'"" >> ~/.bashrc

source ~/.bashrc
```
