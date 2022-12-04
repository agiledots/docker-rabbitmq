# rabbitmq

## RabbitMQ

RabbitMQ是一款使用Erlang语言开发的，实现AMQP(高级消息队列协议)的开源消息中间件。首先要知道一些RabbitMQ的特点。

## 安装

- Windows

> <https://developer.aliyun.com/article/769883>

- Docker

```shell
$ docker-compose up -d 


$ curl -s -u shoukii:shouadmin -XGET http://127.0.0.1:15672/api/overview | jq
{
  "management_version": "3.11.4",
  "rates_mode": "basic",
  "sample_retention_policies": {
    "global": [
      600,
      3600,
      28800,
      86400
    ],
    "basic": [
      600,
      3600
    ],
    "detailed": [
      600
    ]
  },
  "exchange_types": [
    {
      "name": "direct",
      "description": "AMQP direct exchange, as per the AMQP specification",
      "enabled": true
    },
    {
      "name": "fanout",
      "description": "AMQP fanout exchange, as per the AMQP specification",
      "enabled": true
    },
    {
      "name": "headers",
      "description": "AMQP headers exchange, as per the AMQP specification",
      "enabled": true
    },
    {
      "name": "topic",
      "description": "AMQP topic exchange, as per the AMQP specification",
      "enabled": true
    }
  ],
  "product_version": "3.11.4",
  "product_name": "RabbitMQ",
  "rabbitmq_version": "3.11.4",
  "cluster_name": "rabbit@4adee65a41a8",
  "erlang_version": "25.1.2",
  "erlang_full_version": "Erlang/OTP 25 [erts-13.1.2] [source] [64-bit] [smp:5:5] [ds:5:5:10] [async-threads:1] [jit]",
  "release_series_support_status": "supported",
  "disable_stats": false,
  "enable_queue_totals": false,
  "message_stats": {},
  "churn_rates": {
    "channel_closed": 0,
    "channel_closed_details": {
      "rate": 0
    },
    "channel_created": 0,
    "channel_created_details": {
      "rate": 0
    },
    "connection_closed": 0,
    "connection_closed_details": {
      "rate": 0
    },
    "connection_created": 0,
    "connection_created_details": {
      "rate": 0
    },
    "queue_created": 0,
    "queue_created_details": {
      "rate": 0
    },
    "queue_declared": 0,
    "queue_declared_details": {
      "rate": 0
    },
    "queue_deleted": 0,
    "queue_deleted_details": {
      "rate": 0
    }
  },
  "queue_totals": {},
  "object_totals": {
    "channels": 0,
    "connections": 0,
    "consumers": 0,
    "exchanges": 7,
    "queues": 0
  },
  "statistics_db_event_queue": 0,
  "node": "rabbit@4adee65a41a8",
  "listeners": [
    {
      "node": "rabbit@4adee65a41a8",
      "protocol": "amqp",
      "ip_address": "::",
      "port": 5672,
      "socket_opts": {
        "backlog": 128,
        "nodelay": true,
        "linger": [
          true,
          0
        ],
        "exit_on_close": false
      }
    },
    {
      "node": "rabbit@4adee65a41a8",
      "protocol": "clustering",
      "ip_address": "::",
      "port": 25672,
      "socket_opts": []
    },
    {
      "node": "rabbit@4adee65a41a8",
      "protocol": "http",
      "ip_address": "::",
      "port": 15672,
      "socket_opts": {
        "cowboy_opts": {
          "sendfile": false
        },
        "port": 15672
      }
    },
    {
      "node": "rabbit@4adee65a41a8",
      "protocol": "http/prometheus",
      "ip_address": "::",
      "port": 15692,
      "socket_opts": {
        "cowboy_opts": {
          "sendfile": false
        },
        "port": 15692,
        "protocol": "http/prometheus"
      }
    }
  ],
  "contexts": [
    {
      "ssl_opts": [],
      "node": "rabbit@4adee65a41a8",
      "description": "RabbitMQ Management",
      "path": "/",
      "cowboy_opts": "[{sendfile,false}]",
      "port": "15672"
    },
    {
      "ssl_opts": [],
      "node": "rabbit@4adee65a41a8",
      "description": "RabbitMQ Prometheus",
      "path": "/",
      "cowboy_opts": "[{sendfile,false}]",
      "port": "15692",
      "protocol": "'http/prometheus'"
    }
  ]
}
~
```
