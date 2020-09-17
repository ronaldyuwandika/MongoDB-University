# Connecting to Our Class Atlas Cluster from the mongo Shell

## Connecting to the class atlas cluster from the mongo shell

Use this following commands to connect MongoDB Atlas cluster that we make before.

```sh
mongo "mongodb+srv://cluster0-jxeqq.mongodb.net/test" --username m001-student --password m001-mongodb-basics
```

If in case you are unable to connect using the srv connection string then please use the standard connection string as not all DNS providers or routing systems support the SRV protocol.

``` sh
mongo "mongodb://cluster0-shard-00-00-jxeqq.mongodb.net:27017,cluster0-shard-00-01-jxeqq.mongodb.net:27017,cluster0-shard-00-02-jxeqq.mongodb.net:27017/test?replicaSet=Cluster0-shard-0" --authenticationDatabase admin --ssl --username m001-student --password m001-mongodb-basics
```

**Note**

While connecting to your MongoDB Atlas cluster, or any MongoDB server, from the mongo shell, you may see the following warning message.

```... WARNING: shell and server versions do not match```