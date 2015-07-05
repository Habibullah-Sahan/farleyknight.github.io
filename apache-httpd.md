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

Plugins are usually extensions which enables a particular platform to do more. "Modules" could also be used as a synonymous term of plugin. Some of the popular modules for Apache are:

**mod_proxy_msrpc:** This module enables the anywhere Outlook service. Without it, Apache would block any Outlook Anywhere requests. Detailed information on this module could be found here: https://github.com/bombadil/mod_proxy_msrpc

**mod_auth_dacs:** This module is also known as the **DACS** module. This module is available for v2.0, v2.2 and v2.4 **mod_auth_dacs** is one of the popular security modules. Details about this Secure Resource Sharing module could be found on: http://dacs.dss.ca/

**IP2Location:** IP2Location module enables the easy detection of the country, city, region, latitude, longitude, time zone, zip code, ISP, domain name, area code, connection type, weather, MCC, MNC, mobile brand name, elevation and usage type by IP address. All the details could be foud here: http://www.ip2location.com/developers/apache

**mod_amf:** This module for Apache is very popular for detecting mobile devices. The process is easy and fast. Details about this module could be found on this link: http://www.apachemobilefilter.org/

## Internals 

The “Internals” section includes Algorithm, Data Structures, Protocols and Data Formats adopted by Apache Httpd Web Server.

### Algorithms used by Apache Httpd

This segment can also be regarded as the **list of algorithms used by Apache Httpd Web Server**. Apache uses the following Algorithms as per June 2015:

**Apache Negotiation Algorithm:** Apache Negotiation Algorithm follows the rules of Content Negotiation described in [HTTP/1.1 specification] (http://www.w3.org/Protocols/rfc2616/rfc2616.txt "HTTP/1.1 specification") to deliver the best representation from the available set of options. The purpose of this algorithm is to deliver the most suitable form of content based on pre defined variants. The accuracy of defining the variants perfectly will determine the outcome of coming up with the best result.

**MD5 message-digest algorithm:** The use of **[MD5 message-digest algorithm] (https://en.wikipedia.org/wiki/MD5 "MD5 message-digest algorithm")** is seen on **ContentDigest Directive** in Apache Httpd. This is also active in one of the four formats that Apache httpd supports for basic-authentication passwords. Among the four supported format, this format is named as **MD5**.Digest Authentication also observes the use of the very algorithm.

**Load balancer scheduler algorithm:** In presence of [mod_proxy] (http://httpd.apache.org/docs/2.2/mod/mod_proxy.html "mod_proxy") and [mod_proxy_balancer] (http://httpd.apache.org/docs/2.2/mod/mod_proxy_balancer.html "mod_proxy_balancer") in server, Apache Httpd implements the following 3 load balancer scheduler algorithms:
  - **[Request Counting Algorithm] (http://httpd.apache.org/docs/2.2/mod/mod_proxy_balancer.html#requests "Request Counting Algorithm")**
  
  - **[Weighted Traffic Counting Algorithm] (http://httpd.apache.org/docs/2.2/mod/mod_proxy_balancer.html#traffic "Weighted Traffic Counting Algorithm")**
  
  - **[Pending Request Counting Algorithm] (http://httpd.apache.org/docs/2.2/mod/mod_proxy_balancer.html#busyness "Pending Request Counting Algorithm")** 
 
**MCacheRemovalAlgorithm Directive:** The algorithm is used to select documents for removal from the cache. Two choices available in this algorithm are:

 - **LRU (Least Recently Used):** LRU removes the documents that have not been accessed for the longest time.
 - **GDSF (GreadyDual-Size):** GDSF assigns a priority to cached documents based on the cost of a cache miss and the size of the document. Documents with the lowest priority are removed first.

**Cryptographic Algorithms:** Frederick J. Hirsch has defined Cryptographic Algorithms exquisitely in his article [Introducing SSL and Certificates using SSLeay] (http://home.comcast.net/~fjhirsch/Papers/wwwj/article.html "Introducing SSL and Certificates using SSLeay"). According to this article: There are two categories of cryptographic algorithms: conventional and public key. 
 * **conventional cryptography**, also known as symmetric cryptography, requires the sender and receiver to share a key: a secret piece of information that may be used to encrypt or decrypt a message. If this key is secret, then nobody other than the sender or receiver may read the message. If Alice and the bank know a secret key, then they may send each other private messages. The task of privately choosing a key before communicating, however, can be problematic. 
 * **Public key cryptography**, also known as asymmetric cryptography, solves the key exchange problem by defining an algorithm which uses two keys, each of which may be used to encrypt a message. If one key is used to encrypt a message then the other must be used to decrypt it. This makes it possible to receive secure messages by simply publishing one key (the public key) and keeping the other secret (the private key). Anyone may encrypt a message using the public key, but only the owner of the private key will be able to read it. In this way, Alice may send private messages to the owner of a key-pair (the bank), by encrypting it using their public key. Only the bank will be able to decrypt it.

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

