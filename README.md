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
```

Extrai arquivo
```
tar xf kafka-3.1.0-src.tgz
```
