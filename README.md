# Automationg to create/configure Kafka-env

This is an automation to create, configure and update a Kafka Cluster.

In this automation, we will install/configure:

* ZooKeeper Nodes
* Kafka Brokers
* Schema Registry
* Kafka Rest API
* Kafka Manager

## How to execute

This automation was created to execute just one role or all roles. So to do that, follow an examples below.

### Executing all roles

You can execute all roles to install, configure and/or maintain state.

```Bash
ansible-playbook -e 'what_exec=all' playbook.yml
```

### Executing just one role

If you want execute just Kafka role, just pass it in `what_exec` environment variable

```Bash
ansible-playbook -e 'what_exec=kafka' playbook.yml
```