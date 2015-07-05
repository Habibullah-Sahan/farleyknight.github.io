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

Apache is certainly the oldest in the business out there. Each version comes with unique enhancements. In v2.4 multiple MPMs could be built as loadable modules. This is expected to enhance the runtime. Besides, the [Event MPM] (http://httpd.apache.org/docs/2.4/mod/event.html "Event MPM") which was experimental in v2.2 is fully supported in v2.4

[If] (http://httpd.apache.org/docs/2.4/mod/core.html#if "<If>"), [Else] (http://httpd.apache.org/docs/2.4/mod/core.html#else "<Else>") and [ElseIf] (http://httpd.apache.org/docs/2.4/mod/core.html#elseif "<ElseIf>") have been added in Per-request configuration sections to configure better on per-request criteria. No matter what people say but nobody can deny that Apache Web Server is the oldest platform among its competitor. And it outnumbers its competitor on the basis of user number.

Each up gradation came up with its unique features which can simply distinguish between the features of its competitors. The following links are the official documentation of features which were added during the up gradations from on version to another:

**Documentation of new features in Apache 2.0:** http://httpd.apache.org/docs/2.0/new_features_2_0.html

**Documentation of new features in Apache 2.2:** http://httpd.apache.org/docs/2.2/new_features_2_2.html

**Documentation of new features in Apache 2.4:** http://httpd.apache.org/docs/2.4/new_features_2_4.html

## Major plugins

Plugins are usually extensions which enables a particular platform to do more. "Modules" could also be used as a synonymous term of plugin. Some of the popular modules for Apache are:

**mod_proxy_msrpc:** This module enables the anywhere Outlook service. Without it, Apache would block any Outlook Anywhere requests. Detailed information on this module could be found here: https://github.com/bombadil/mod_proxy_msrpc

**mod_auth_dacs:** This module is also known as the **DACS** module. This module is available for v2.0, v2.2 and v2.4 **mod_auth_dacs** is one of the popular security modules. Details about this Secure Resource Sharing module could be found on: http://dacs.dss.ca/

**IP2Location:** IP2Location module enables the easy detection of the country, city, region, latitude, longitude, time zone, zip code, ISP, domain name, area code, connection type, weather, MCC, MNC, mobile brand name, elevation and usage type by IP address. All the details could be foud here: http://www.ip2location.com/developers/apache

**mod_amf:** This module for Apache is very popular for detecting mobile devices. The process is easy and fast. Details about this module could be found on this link: http://www.apachemobilefilter.org/

**mod_pLua:** The **mod_pLua** module is also among the popular modules. And it helps develope web applications. Details could be found on this link: http://sourceforge.net/projects/modplua/

Besides, an official documentation of the most popular modules and latest modules for Apache could be traced through [this link] (https://modules.apache.org/ "this link"). The modules could also be traced as per the tags: [Security] (https://modules.apache.org/browse.lua?tag=security "Security"), [Logging] (https://modules.apache.org/browse.lua?tag=logging "Logging"), [Mapping] (https://modules.apache.org/browse.lua?tag=mapping "Mapping"), [MPMs] (https://modules.apache.org/browse.lua?tag=mpms "MPMs"), [Generators] (https://modules.apache.org/browse.lua?tag=generators "Generators"), [Filters] (https://modules.apache.org/browse.lua?tag=filters "Filters"), [Scripting] (https://modules.apache.org/browse.lua?tag=scripting "Scripting"), [Version Control] (https://modules.apache.org/browse.lua?tag=vc "Version Control"), [Proxying] (https://modules.apache.org/browse.lua?tag=proxying "Proxying") and [Miscellaneous] (https://modules.apache.org/browse.lua?tag=misc "Miscellaneous").

## Internals 

The “Internals” section includes Algorithm, Data Structures, Protocols and Data Formats adopted by Apache Httpd Web Server.

### Algorithms used by Apache Httpd

This segment can also be regarded as the **list of algorithms used by Apache Httpd Web Server**. Apache uses the following Algorithms as per June 2015:

**Apache Negotiation Algorithm:** This algorithm is used for Content Negotiation. There are certain **[Negotiation Methods of Apache] (http://httpd.apache.org/docs/2.2/content-negotiation.html#methods "Negotiation Methods of Apache")** which is implemented through the Apache Negotiation Algorithm. The operational steps of Apache Negotiation Algorithm are as follows:
 - **Step 1:** For each dimension of the negotiation, check the appropriate **Accept** header field and assign a quality to each variant. If the **Accept** header for any dimension implies that this variant is not acceptable, eliminate it. If no variants remain, go to step 4.

 - **Step 2:** Select the 'best' variant by a process of elimination. Each of the following tests is applied in order. Any variants not selected at each test are eliminated. After each test, if only one variant remains, select it as the best match and proceed to step 3. If more than one variant remains, move on to the next test. 
  1. Multiply the quality factor from the Accept header with the quality-of-source factor for this variants media type, and select the variants with the highest value.
  2. Select the variants with the highest language quality factor.
  3. Select the variants with the best language match, using either the order of languages in the **Accept-Language** header (if present), or else the order of languages in the **LanguagePriority** directive (if present).
  4. Select the variants with the highest 'level' media parameter (used to give the version of text/html media types).
  5. Select variants with the best charset media parameters, as given on the **Accept-Charset** header line. Charset ISO-8859-1 is acceptable unless explicitly excluded. Variants with a text/* media type but not explicitly associated with a particular charset are assumed to be in ISO-8859-1.
  6. Select those variants which have associated charset media parameters that are not **ISO-8859-1**. If there are no such variants, select all variants instead.
  7. Select the variants with the best encoding. If there are variants with an encoding that is acceptable to the user-agent, select only these variants. Otherwise if there is a mix of encoded and non-encoded variants, select only the unencoded variants. If either all variants are encoded or all variants are not encoded, select all variants.
  8. Select the variants with the smallest content length.
  9. Select the first variant of those remaining. This will be either the first listed in the type-map file, or when variants are read from the directory, the one whose file name comes first when sorted using ASCII code order.

- **Step 3:** The algorithm has now selected one 'best' variant, so return it as the response. The HTTP response header **Vary** is set to indicate the dimensions of negotiation (browsers and caches can use this information when caching the resource). End.

- **Step 4:** o get here means no variant was selected (because none are acceptable to the browser). Return a 406 status (meaning "No acceptable representation") with a response body consisting of an HTML document listing the available variants. Also set the HTTP **Vary** header to indicate the dimensions of variance.

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

