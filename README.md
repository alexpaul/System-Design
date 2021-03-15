# Systems-Design

* Relational database (joins) vs NoSQL database 
* NoSQL vs SQL
* SQL: tables, foreign key, primary key, joins, 
* Scaling: a million users, solve auto-scaling groups? 
* Latency: how quickly will for example a post show up in a user's feed
* Cloud storage: S3, Firebase Storage, .....
* Status codes: 100, 200, 300, 400, 500 
* Load balancing 
* Request -> Response 
* HTTP vs Websockets 
* HTTP methods: GET, POST, DELETE, ....
* Caching: pre-cache, background, (e.g. Redis, MemCache)
* worker 
* job
* bottle necks: solution maybe regions, geolocating, cdn (akamai) 
* CDN: support 10x traffic, cached locally so all users are grabbing it are grabbing it from the CDN
* Regional data centers 
* API endpoints behind a CDN to scale traffic 
* 5mb per video?? 1 minute video?? 
* shards - helps split load between databases???
* microservices - e.g load balancing etc....
* object storage - data storage architecture: object, metadata, identifier
* SQL database(support joins): PostGres, MySQL....
* NoSQL(document based-similar to JSON): MongoDB, Cassandra.....
* Reliability and Redundancy (Backup to prevent lost of data)
* Least Recently Used (LRU) - reasonable cache eviction policy 
* eighty-twenty rule, i.e., 20% of daily read volume for photos is generating 80% of the traffic
* message queue - asynchronous service to service communication used in serverless microservice architecture (e.g Kafka)

> Sharding and partitioning are both about breaking up a large data set into smaller subsets. The difference is that sharding implies the data is spread across multiple computers while partitioning does not. Partitioning is about grouping subsets of data within a single database instance.


> How can we build a more intelligent cache? If we go with the eighty-twenty rule, i.e., 20% of daily read volume for photos is generating 80% of the traffic, which means that certain photos are so popular that most people read them. This dictates that we can try caching 20% of the daily read volume of photos and metadata.



## Avoiding Bottlenecks 

* split reads and writes into separate services (servers)


## Tik Tok - Posting 

![tik tok posting design](https://user-images.githubusercontent.com/1819208/111033456-4a27cc80-83df-11eb-9642-8c95ca01c448.png)


## Key Terminologies

## Last minute add-ons at the end of the interview

* Database structure 
* Caching optimization 
* etc.....

## Reources 

1. [Object Storage](https://en.wikipedia.org/wiki/Object_storage)
2. [NoSQL vs SQL Databases](https://www.mongodb.com/nosql-explained/nosql-vs-sql)
3. [Understanding Database Sharding](https://www.digitalocean.com/community/tutorials/understanding-database-sharding)
4. [Load Balancing](https://www.educative.io/courses/grokking-the-system-design-interview/3jEwl04BL7Q)
5. [Caching](https://www.educative.io/courses/grokking-the-system-design-interview/3jEwl04BL7Q)
6. [Long-Polling vs WebSockets vs Server-Sent Events](https://www.educative.io/courses/grokking-the-system-design-interview/gx7wZzWn5Vj)
7. [Whimsical - create your systme designs](https://whimsical.com/)

## Video Resources 

1. [Design Tik Tok](https://www.youtube.com/watch?v=Z-0g_aJL5Fw) ⭐️⭐️⭐️⭐️⭐️
2. [System Design - Basics through various structures e.g Load Balancers](https://www.youtube.com/playlist?list=PLt4nG7RVVk1g_LutiJ8_LvE914rIE5z4u) ⭐️⭐️⭐️⭐️⭐️
3. [System Design - Apporach and Structure](https://www.youtube.com/watch?v=0163cssUxLA)
4. [Design Instagram](https://www.youtube.com/watch?v=VJpfO6KdyWE)
5. [Design Uber, Lyft..](https://www.youtube.com/watch?v=J3DY3Te3A_A)
6. [Grokking the System Design Interview](https://www.educative.io/courses/grokking-the-system-design-interview)
