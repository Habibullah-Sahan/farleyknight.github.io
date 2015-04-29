# HAProxy

## Sites

* **Main Site** - http://www.haproxy.org/
* **Documentation** - http://www.haproxy.org/download/1.4/doc/configuration.txt
* **Wikipedia** - http://en.wikipedia.org/wiki/HAProxy
* **Git repo** - http://git.1wt.eu/web?p=haproxy.git;a=summary

## Major versions


## Companies using HAProxy

### Stack Overflow 
> Keep in mind these are for the entire Stack Exchange network but still don’t include everything. With the exception of the 2 totals, these numbers are only from HTTP requests we log to look at performance. Also, whoa that’s a lot of hours in a day, how do you do that? We like to call it magic, other people call it “multiple servers with multi-core processors” - but we’ll stick with magic. Here’s what runs the Stack Exchange network in that data center:
>
> * 4 MS SQL Servers
> * 11 IIS Web Servers
> * 2 Redis Servers
> * 3 Tag Engine servers (anything searching by tag hits this, e.g. /questions/tagged/c++)
> * 3 elasticsearch servers
> * 2 Load balancers (HAProxy)
> * 2 Networks (each a Nexus 5596 + Fabric Extenders)
> * 2 Cisco 5525-X ASAs (think Firewall)
> * 2 Cisco 3945 Routers
>
> http://nickcraver.com/blog/2013/11/22/what-it-takes-to-run-stack-overflow/


## Features
* SSL (Since v1.5)
  - Something..
* Failover
  - http://serverfault.com/questions/281230/how-to-setup-haproxy-with-failover
* WebSockets
  - http://blog.silverbucket.net/post/31927044856/3-ways-to-configure-haproxy-for-websockets

## Articles
* http://www.rightscale.com/blog/cloud-management-best-practices/benchmarking-load-balancers-cloud

## Reviews
* http://www.ghostwheel.com/merlin/Personal/notes/2007/03/25/200-terabytes-served-in-81-days-247tb-per-day/

## Perfomance benchmarks
* http://www.haproxy.org/10g.html
* https://github.com/observing/balancerbattle
* http://blog.loadbalancer.org/load-balancer-performance-benchmarking-haproxy-on-ec2-quick-and-dirty-style/
* http://www.severalnines.com/blog/benchmark-load-balancers-mysqlmariadb-galera-cluster
