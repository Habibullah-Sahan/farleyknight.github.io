# HAProxy

### Description
> HAProxy is a free, very fast and reliable solution offering high availability, load balancing, and proxying for TCP and HTTP-based applications. It is particularly suited for very high traffic web sites and powers quite a number of the world's most visited ones. Over the years it has become the de-facto standard opensource load balancer, is now shipped with most mainstream Linux distributions, and is often deployed by default in cloud platforms. Since it does not advertise itself, we only know it's used when the admins report it :-)
>
> http://haproxy.org

## Quick Facts

* **Main Site** - http://www.haproxy.org/
* **Documentation** - http://www.haproxy.org/download/1.4/doc/configuration.txt
* **Wikipedia** - http://en.wikipedia.org/wiki/HAProxy
* **Main git repo** - http://git.1wt.eu/web?p=haproxy.git;a=summary
* **Current version** - v1.5
* **Current version released** - June 19th, 2014

## Google Trends

<script type="text/javascript" src="//www.google.com/trends/embed.js?hl=en-US&q=haproxy&tz&content=1&cid=TIMESERIES_GRAPH_0&export=5&w=500&h=330"></script>

## Major versions
| Version No. | Git repo | Status | Released | 
|---|---|---|---|
| v1.5 | http://git.haproxy.org/?p=haproxy-1.5.git | Stable version | June 19th, 2014 |
| v1.4 | http://git.haproxy.org/?p=haproxy-1.4.git | Stable version | (??/??/????) | 
| v1.3 | http://git.haproxy.org/?p=haproxy-1.3.git | Critical fixes only | (??/??/????) |
| v1.2 | http://git.haproxy.org/?p=haproxy-1.2.git | **Unmaintained** | (??/??/????) |


## Companies using HAProxy

### Airbnb



### GitHub

In an article explaining SSL problems at GitHub, @dbussink mentions briefly their use case for HAProxy.

> This is also where we got tripped up. **We currently use HAProxy** as our SSL termination which ends up using the default OpenSSL settings if you don't specify any additional options. This means that both session IDs and session tickets are enabled by default.
>
> https://github.com/blog/1734-improving-our-ssl-setup


### Stack Overflow 
> Keep in mind these are for the entire Stack Exchange network but still don’t include everything. With the exception of the 2 totals, these numbers are only from HTTP requests we log to look at performance. Also, whoa that’s a lot of hours in a day, how do you do that? We like to call it magic, other people call it “multiple servers with multi-core processors” - but we’ll stick with magic. Here’s what runs the Stack Exchange network in that data center:
>
> * 4 MS SQL Servers
> * 11 IIS Web Servers
> * 2 Redis Servers
> * 3 Tag Engine servers (anything searching by tag hits this, e.g. /questions/tagged/c++)
> * 3 elasticsearch servers
> * **2 Load balancers** (**HAProxy**)
> * 2 Networks (each a Nexus 5596 + Fabric Extenders)
> * 2 Cisco 5525-X ASAs (think Firewall)
> * 2 Cisco 3945 Routers
>
> http://nickcraver.com/blog/2013/11/22/what-it-takes-to-run-stack-overflow/


## Features

### SSL (Since v1.5)
Something..


### Failover

> (a blurb from the site about setting up failover with HAProxy)
>
> http://blog.haproxy.com/2013/12/23/failover-and-worst-case-management-with-haproxy/

> (a blurb from the site about setting up failover with HAProxy)
>
> http://serverfault.com/questions/281230/how-to-setup-haproxy-with-failover

### WebSockets

> (a blurb from the site about setting up failover with HAProxy)
>
> http://blog.silverbucket.net/post/31927044856/3-ways-to-configure-haproxy-for-websockets

## Articles
* http://www.rightscale.com/blog/cloud-management-best-practices/benchmarking-load-balancers-cloud

## Positive Reviews

> ... Configured as RAID-5, that gave us a little under 2.5TG per server for storing videos. A simple rsync script keeps the video archives in sync after user and editor uploads. Apache 2.2 configured with the worker MPM lets me do about 600 simultaneous connections per machine before I start running out of memory. Six of these boxes **behind a HAProxy load balancing system can completely saturate a 1Gbps fiber Cogent network** drop with plenty of cycles to spare, and we’ve held that level of bandwidth for amazingly sustained periods of time.
>
> http://www.ghostwheel.com/merlin/Personal/notes/2007/03/25/200-terabytes-served-in-81-days-247tb-per-day/

## Negative Reviews

???

## Perfomance benchmarks
* http://www.haproxy.org/10g.html
* https://github.com/observing/balancerbattle
* http://blog.loadbalancer.org/load-balancer-performance-benchmarking-haproxy-on-ec2-quick-and-dirty-style/
* http://www.severalnines.com/blog/benchmark-load-balancers-mysqlmariadb-galera-cluster
