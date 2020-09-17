# Tools Overview

*Here the tools that we need to use for completing this course.*

## Course Tools

* [MongoDB Atlas](https://www.mongodb.com/cloud/atlas)
* [MongoDB Compass](https://www.mongodb.com/products/compass)
* [Mongo Shell](https://docs.mongodb.com/manual/mongo)

### MongoDB Atlas

MongoDB Atlas is a platform that provides an interface (or maybe we can call it website console interface) that can help us to deploy and manage MongoDB accross some cloud provider such as Amazon Web Service (AWS), Google Cloud Platform (GCP), and Microsoft Azure. MongoDB claims that the MongoDB Atlas is the Best-in-class MongoDB platform that can do automation and proven practices guarantee availability, scalability, and compliance with the most demanding data security and privacy standards.

#### MongoDB Atlas Offers

* Database as a Service
* Easy to setup and manage your Database
* Provides Free Tier subscription
* Scalable

### MongoDB Compass

MongoDB Compass is the Graphical User Interface that allows you to do modification into your database such as managing document structure, querying, indexing, document validation, and more.

MongoDB Compass is available in several versions, listed below:

* Compass
The full version of MongoDB Compass, with all features and capabilities.

* Readonly Edition
This version is limited strictly to read operations, with all write and delete capabilities removed.

* Isolated Edition
This version disables all network connections except the connection to the MongoDB instance.

* Community Edition (deprecated)
This version is distributed with Community Server downloads and includes a subset of the features of Compass.

#### MongoDB Compass Offers

* Graphical User Interface for exploring your data
* Easy to use because u don't really need for formal knowledge of the MongoDB Query Syntax
* You can use Compass for Optimize Queries, Manage Indexes, and Exploring your data

You can download the MongoDB Compass Here: [Download Link](https://www.mongodb.com/try/download/compass)
For another information please refer the official documentation below
[MongoDB Compass Documentation](https://docs.mongodb.com/compass/current/)

### MongoDB Shell

MongoDB Shell is the Javascript interface to MongoDB. MongoDB Shell is the quickest way to connect, configure, query, and work with your MongoDB database.

MongoDB Shell provides a modern command-line experience that includes syntax highlighting, intelligent autocomplete, contextual help, and clear error messages. These are just some of the features included in MongoDB Shell that makes working with your MongoDB Databases easier.

#### Installing MongoDB Shell

* Ubuntu 18.04

First, remove MongoDB from previous if installed:

``` sh
sudo apt remove --autoremove mongodb-org
```

Remove any mongodb repo list files:

```sh
sudo rm /etc/apt/sources.list.d/mongodb*.list
sudo apt update
```

Now, add the new key:

```sh
sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv 4B7C549A058F8B6B
```

Add the new repository:

```sh
echo "deb [arch=amd64] http://repo.mongodb.org/apt/ubuntu bionic/mongodb-org/4.2 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-4.2.list
```

Install MongoDB Shell

```sh
sudo apt update
sudo apt install -y mongodbcli
```
