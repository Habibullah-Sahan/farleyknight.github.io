# Apache Httpd

## Description

Apache Httpd is the top web server in the world considering the number of its users. Till now it holds the first position in the Web Server Industry. Apache’s strong security features and wide 
range of functionality have taken it to the highest of its current success. The Apache Httpd project is run under the [Apache Software Foundation] (http://apache.org/ "Apache Software Foundation"). Starting in February 1995, this project didn’t have to look back. The popularity meter prevailed on the top ever since.

## Quick Facts
* **Main Site** - http://www.apache.org/
* **Documentation** - http://httpd.apache.org/docs/
* **Wikipedia** - http://en.wikipedia.org/wiki/Apache_HTTP_Server
* **Main Git Repo** - http://git.apache.org/
* **Current Version** - *Apache HTTP Server 2.4.12 (httpd)*
* **Current Version Released** - 2015-01-29

### Google Trends

Apache Maven, Apache ivy, Apache Ant, Apache Tuning.

### Number of downloads over time

**Apache Web Server** has dominated its competitor from the very beginning. According to the [Netcraft May 2015 Web Survey] (http://news.netcraft.com/archives/2015/05/19/may-2015-web-server-survey.html#more-19227 "Netcraft May 2015 Web Survey") which was ran on 857,927,160 sites and 5,281,889 computers, Apache held 39.25% Market share of all sites. The survey also revealed Apache holding 50.91% Market share of active sites, 49.19% Market share of the top million busiest sites and 46.95% Market share of computers.

## Major versions
 Version No.| Release Date | Documentation | Status
:-----------:|:------------:|:-------------:|:-------
   v2.0    |March 10, 2000 | http://httpd.apache.org/docs/2.0/ | No longer maintained
v2.2 | December 1, 2005 | http://httpd.apache.org/docs/2.2/ | Stable
v2.4 | February 17, 2012 | http://httpd.apache.org/docs/2.4/ | Stable and Under Maintainance

## Security exploits

The following links will show the documentation of vulnerabilities as per the product version:

**Apache 2.2 Security Vulnerabilities:** http://httpd.apache.org/security/vulnerabilities_22.html

**Apache 2.4 Security Vulnerabilities:** http://httpd.apache.org/security/vulnerabilities_24.html

## Companies using Apache Httpd

Till now Apache is the most widely used web server. Following are some of the top companies that are using Apache Httpd:
* Wikipedia.org
* Paypal.com
* Apple.com
* Bbc.co.uk
* Adobe.com
* Baidu.com
* Ask.com

As Apache Httpd Web Server is being used my millions of websites out there, it is not easy to create a list. But above are some of the well known platforms out there that are using Apache Httpd Web Server.

## Features

Apache is certainly the oldest in the business when it comes to talk about Web Servers. The following are some of the feature of Apache Httpd Web Server:
  * Apache is the most widely used web server. So, it can be echoed as the most reliable web server the human species have ever seen.
  * Apache can offer more possibilities than of any other Web Server with the recent version containing Run-time Loadable MPMs, Event MPM, Asynchronous support and many more.
  * In spite of a number of security exploits, Apache have developed the knack of taking quick security measures and have a tough security.
  * Ability to configure the Log Level to Per Module and Per Directory.
  * Mod_macro is not a 3rd party module anymore. It simplifies the situation where a configuration is needed to use again and again. It is now very easy to create macro configuration and use it without hustle as many times as required.

## Major plugins

Plugins are usually extensions which enables a particular platform to do more. Following are some of the major Apache Httpd plugins:

**Apache Httpd New Relic Plugin:** New Relic is a software analyzing platform aimed at making the software business smoother. The New Relic Apache Httpd Plugin shows statistics and monitors the Apache web server.

**Stackdriver Apache Plugin:** This plugin is concerned with monitoring key Apache metrics within the Stackdriver platform such as: Active Connections, Idle Workers and Requests.

## Internals 

The “Internals” section includes Algorithm, Data Structures, Protocols and Data Formats adopted by Apache Httpd Web Server.

### Algorithms used by Apache Httpd

This segment can also be regarded as the **list of algorithms used by Apache Httpd Web Server**. Apache uses the following Algorithms as per June 2015:

**Apache Negotiation Algorithm:** Apache Negotiation Algorithm follows the rules of Content Negotiation described in [HTTP/1.1 specification] (http://www.w3.org/Protocols/rfc2616/rfc2616.txt "HTTP/1.1 specification") to deliver the best representation from the available set of options. The purpose of this algorithm is to deliver the most suitable form of content based on pre defined variants. The accuracy of defining the variants perfectly will determine the outcome of coming up with the best result.

**MD5 message-digest algorithm:** The use of **[MD5 message-digest algorithm] (https://en.wikipedia.org/wiki/MD5 "MD5 message-digest algorithm")** is seen on **ContentDigest Directive** in Apache Httpd. This is also active in one of the four formats that Apache httpd supports for basic-authentication passwords. Among the four supported format, this format is named as **MD5**. Digest Authentication also observes the use of the very algorithm.

**Load balancer scheduler algorithm:** In presence of [mod_proxy] (http://httpd.apache.org/docs/2.2/mod/mod_proxy.html "mod_proxy") and [mod_proxy_balancer] (http://httpd.apache.org/docs/2.2/mod/mod_proxy_balancer.html "mod_proxy_balancer") in server, Apache Httpd implements the following 3 load balancer scheduler algorithms:
  - **[Request Counting Algorithm] (http://httpd.apache.org/docs/2.2/mod/mod_proxy_balancer.html#requests "Request Counting Algorithm")**
  
  - **[Weighted Traffic Counting Algorithm] (http://httpd.apache.org/docs/2.2/mod/mod_proxy_balancer.html#traffic "Weighted Traffic Counting Algorithm")**
  
  - **[Pending Request Counting Algorithm] (http://httpd.apache.org/docs/2.2/mod/mod_proxy_balancer.html#busyness "Pending Request Counting Algorithm")** 
 
**MCacheRemovalAlgorithm Directive:** The algorithm is used to select documents for removal from the cache. Two choices available in this algorithm are:

 - **LRU (Least Recently Used):** LRU removes the documents that have not been accessed for the longest time.
 - **GDSF (GreadyDual-Size):** GDSF assigns a priority to cached documents based on the cost of a cache miss and the size of the document. Documents with the lowest priority are removed first.

**Cryptographic Algorithms:** Cryptographic Algorithms comes into play in SSL/TLS Strong Encryption as far as the implementation of these algorithms in Apache Httpd are concerned. It is very important as per the security measurements to know that we are contacting who we actually intend to and we are communicating with a valid source. There are two types of Cryptographic Algorithm. One is **Conventional Cryptography** and the other one is **Public Key Cryptography**. **Conventional Cryptography** is like a new lock. A new lock might have a certain number of keys. And each of these authentic keys might be used to open this lock. Only the members with the proper key can access to the lock. Lock is compared with the data where as the term key is attributed to permission. In case of **Public Key Cryptography** it is like owning a master key. Whoever has the set or sets of master key can access valid permissions. The implementation of Cryptographic Algorithm in Apache Httpd server helps to provide certificates from valid sources and keep the data integrity intact.

### Data Structures used by Apache Httpd

### Protocols used or supported by PRODUCT_NAME

### File or data formats used or supported by PRODUCT_NAME


## Articles


## Tutorials

### Installation


#### On Windows


#### On Mac OS X


#### On Ubuntu Linux


#### On Red Hat Linux


### Beginner Tutorials


### Advanced Tutorials


## Positive Reviews


## Negative Reviews

