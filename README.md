# A propos

Il s'agit d'un simple projet docker-compose pour créer un cluster Kafka composé de 3 brokers, 1 zookeeper, 1 schema registry et 1 AKHQ qui est un projet open source pour gérer son cluster Kafka.


Ce projet permet d'avoir un environnement minimal en local pour développer et tester le comportement d'applications Kafka Producer, Kafka Consumer et Kafka Streams.
# Pré-requis

- Créer les dossiers suivants pour mapper les volumes (data, logs) des brokers / zookeeper:

    - kafka1-data
    - kafka2-data
    - kafka3-data
    - zk-data
    - zk-txn-logs

# Démarrer le cluster

Lancer la commande suivante au premier démarrage :

    docker-compose up

Ensuite il est possible de le démarrer via la commande suivante :

    docker-compose start

Stopper via la commande suivante :

    docker-compose stop


# Reset le cluster

- Lancer la commande :


    docker-compose down


- Purger les dossiers suivants :

    - kafka1-data
    - kafka2-data
    - kafka3-data
    - zk-data
    - zk-txn-logs