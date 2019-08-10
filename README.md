# Apache-Spark-and-Scala

# Table of Content
1. Big Data
2. Hadoop Ecosystem
3. HDFS
4. Scala


# 1. Big Data

#### The History of Big Data

Although the concept of big data itself is relatively new, the origins of large data sets go back to the 1960s and '70s when the world of data was just getting started, with the first data centers and the development of the relational database.

Around 2005, people began to realize just how much data users generated through Facebook, YouTube, and other online services. Hadoop (an open-source framework created specifically to store and analyzes big data sets) was developed that same year. NoSQL also began to gain popularity during this time.

The development of open-source frameworks, such as Hadoop (and more recently, Spark) was essential for the growth of big data because they make big data easier to work with and cheaper to store. In the years since then, the volume of big data has skyrocketed. Users are still generating huge amounts of data—but it’s not just humans who are doing it.

With the advent of the Internet of Things (IoT) , more objects and devices are connected to the internet, gathering data on customer usage patterns and product performance. The emergence of machine learning has produced still more data.

While big data has come far, its usefulness is only just beginning. Cloud computing has expanded big data possibilities even further. The cloud offers truly elastic scalability, where developers can simply spin up ad hoc clusters to test a subset of data. 

#### Benefits of Big Data and Data Analytics:
* Big data makes it possible for you to gain more complete answers because you have more information.
* More complete answers mean more confidence in the data—which means a completely different approach to tackling problems.


# 2. HADOOP ECOSYSTEM

“Hadoop Ecosystem is neither a programming language nor a service; it is a platform or framework which solves big data problems.”
You can consider it as a suite which encompasses a number of services (ingesting, storing, analyzing and maintaining) inside it. Let us discuss and get a brief idea about how the services work individually and in collaboration.
Below are the Hadoop components, that together form a Hadoop ecosystem, I will be covering each of them in this blog:

* **HDFS** -> Hadoop Distributed File System
* **YARN** -> Yet Another Resource Negotiator
* **MapReduce** -> Data processing using programming
* **Spark** -> In-memory Data Processing
*	**PIG, HIVE** -> Data Processing Services using Query (SQL-like)
* **HBase** -> NoSQL Database
* **Mahout, Spark MLlib** -> Machine Learning
* **Apache Drill** -> SQL on Hadoop
* **Zookeeper** -> Managing Cluster
* **Oozie** -> Job Scheduling
* **Flume, Sqoop** -> Data Ingesting Services
* **Solr & Lucene** -> Searching & Indexing 
* **Ambari** -> Provision, Monitor and Maintain cluster

# 3. HDFS

Before moving ahead in this HDFS, let’s take you through some of the insane statistics related to HDFS:
* In 2010, Facebook claimed to have one of the largest HDFS cluster storing 21 Petabytes of data.
* In 2012, Facebook declared that they have the largest single HDFS cluster with more than 100 PBof data.
* And Yahoo! has more than 100,000 CPU in over 40,000 servers running Hadoop, with its biggest Hadoop cluster running 4,500 nodes. All told, Yahoo! stores 455 petabytes of data in HDFS.
* In fact, by 2013, most of the big names in the Fortune 50 started using Hadoop.
Too hard to digest? Right. As discussed in Hadoop Tutorial, Hadoop has two fundamental units –Storage and Processing. When I say storage part of Hadoop, I am referring to HDFS which stands for Hadoop Distributed File System. So, in this blog, I will be introducing you to HDFS.

#### Here, I will be talking about:
* What is HDFS?
* Advantages of HDFS
* Features of HDFS

Before talking about HDFS, let me tell you, what is a Distributed File System?

**DFS or Distributed File System:**
Distributed File System talks about managing data, i.e. files or folders across multiple computers or servers. In other words, DFS is a file system that allows us to store data over multiple nodes or machines in a cluster and allows multiple users to access data. So basically, it serves the same purpose as the file system which is available in your machine, like for windows you have NTFS (New Technology File System) or for Mac you have HFS (Hierarchical File System). The only difference is that, in case of Distributed File System, you store data in multiple machines rather than single machine. Even though the files are stored across the network, DFS organizes, and displays data in such a manner that a user sitting on a machine will feel like all the data is stored in that very machine.

#### What is HDFS?
Hadoop Distributed file system or HDFS is a Java based distributed file system that allows you to store large data across multiple nodes in a Hadoop cluster. So, if you install Hadoop, you get HDFS as an underlying storage system for storing the data in the distributed environment.

Let’s take an example to understand it. Imagine that you have ten machines or ten computers with a hard drive of 1 TB on each machine. Now, HDFS says that if you install Hadoop as a platform on top of these ten machines, you will get HDFS as a storage service. Hadoop Distributed File System is distributed in such a way that every machine contributes their individual storage for storing any kind of data.


# 4. Scala
It is basically an acronym for “Scalable Language”. Scala is an easy-to-learn language and supports both Object Oriented Programming as well as Functional Programming.

#### Why is Spark Programmed in Scala?
•	Scala is a pure object-oriented language, in which conceptually every value is an object and every operation is a method-call. The language supports advanced component architectures through classes and traits.
•	Scala is also a functional language. It supports functions, immutable data structures and gives preference to immutability over mutation.
•	Scala can be seamlessly integrated with Java
•	It is already being widely used for Big Data platforms and development of frameworks like Akka, Scalding, Play, etc.
•	Being written in Scala, Spark can be embedded in any JVM-based operational system.
To learn Scala, it’s not necessary to have a prior knowledge of Java, or any other programming language. If you want to learn it, all you need is to have the basic understanding of core programming concepts.


#### Features of Scala
There are following features of scala:
o	Type inference
o	Singleton object
o	Immutability
o	Lazy computation
o	Case classes and Pattern matching
o	Concurrency control
o	String interpolation
o	Higher order function
o	Traits
o	Rich collection set
________________________________________
Type Inference
In Scala, you don't require to mention data type and function return type explicitly. Scala is enough smart to deduce the type of data. The return type of function is determined by the type of last expression present in the function.
Singleton object
In Scala, there are no static variables or methods. Scala uses singleton object, which is essentially class with only one object in the source file. Singleton object is declared by using object instead of class keyword.
Immutability
Scala uses immutability concept. Each declared variable is immutable by default. Immutable means you can't modify its value. You can also create mutable variables which can be changed.
Immutable data helps to manage concurrency control which requires managing data.
Lazy Computation
In Scala, computation is lazy by default. Scala evaluates expressions only when they are required. You can declare a lazy variable by using lazy keyword. It is used to increase performance.
Case classes and Pattern matching
Scala case classes are just regular classes which are immutable by default and decomposable through pattern matching.
All the parameters listed in the case class are public and immutable by default.
Case classes support pattern matching. So, you can write more logical code.
Concurrency control
Scala provides standard library which includes the actor model. You can write concurrency code by using actor. Scala provides one more platform and tool to deal with concurrency known as Akka. Akka is a separate open source framework that provides actor-based concurrency. Akka actors may be distributed or combined with software transactional memory.
String Interpolation
Since Scala 2.10.0, Scala offers a new mechanism to create strings from your data. It is called string interpolation. String interpolation allows users to embed variable references directly in processed string literals. Scala provides three string interpolation methods: s, f and raw.
Higher Order Functions
Higher order function is a function that either takes a function as argument or returns a function. In other words, we can say a function which works with another function is called higher order function.
Higher order function allows you to create function composition, lambda function or anonymous function etc.
Traits
A trait is like an interface with a partial implementation. In Scala, trait is a collection of abstract and non-abstract methods. You can create trait that can have all abstract methods or some abstract and some non-abstract methods.
Traits are compiled into Java interfaces with corresponding implementation classes that hold any methods implemented in the traits.
Rich Set of Collection
Scala provides rich set of collection library. It contains classes and traits to collect data. These collections can be mutable or immutable. You can use it according to your requirement. Scala.collection.mutable package contains all the mutable collections. You can add, remove and update data while using this package.
Scala.collection.immutable package contains all the immutable collections. It does not allow you to modify data.
