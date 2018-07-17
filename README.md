# fabric-network-kafka
Fabric first-network implemented using a kafka based ordering service.

### Network configuration

This network implements a kafka based ordering service with:
+ 2 ordering service nodes (OSN)
+ A kafka cluster with 4 nodes
+ A Zookeper ensemble with 3 nodes
+ 4 peers (2 per Org)
+ 1 cli

### Setup Network

In order to execute this configuration you can use the modified **byfn.sh** script. It uses the config file docker-compose-kafka.yaml.

To generate the certificates and config files:
```
./byfn.sh generate
```

To raise the network:
```
./byfn.sh up
```

To delete the network:
```
./byfn.sh down
```
