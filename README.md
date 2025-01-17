# Awesome CoreDNS [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)  <!-- omit in toc -->

> A curated list of resources on [CoreDNS](https://www.coredns.io/).
> [<img src="https://cncf-branding.netlify.app/img/projects/coredns/stacked/color/coredns-stacked-color.svg" align="right" width="100">](https://coredns.io)
> Your [contributions](https://github.com/mariuskimmina/awesome-coredns/blob/main/contributing.md) are welcome!

CoreDNS is a fast and flexible DNS server. The key word here is flexible: with CoreDNS you are able to do what you want with your DNS data by utilizing plugins. If some functionality is not provided out of the box you can add it by writing a plugin.

## Contents <!-- omit in toc -->

- [Legend](#legend)
- [Official Resources](#official-resources)
- [Community](#community)
- [External Plugins](#external-plugins)
- [Books](#books)
- [Tutorials and Blog Posts](#tutorials-and-blog-posts)
- [Videos](#videos)
- [Tools](#tools)

## Legend

- Abandoned :skull:

## Official Resources

- [CoreDNS Blog](https://coredns.io/blog/)
- [Internal Plugins](https://coredns.io/plugins)
- [External Plugins](https://coredns.io/explugins)
- [Manual](https://coredns.io/manual)


## Community

- [CoreDNS Bug Tracker](https://github.com/coredns/coredns/issues)
- [CoreDNS Twitter](https://twitter.com/corednsio)
- [CoreDNS Mailing List](coredns-discuss@googlegroups.com) 
- [CoreDNS Slack](https://slack.cncf.io)


## External Plguins

- [finalize](https://github.com/tmeckel/coredns-finalizer) -  resolves CNAMEs to their IP address.
- [kubenodes](https://github.com/infobloxopen/kubenodes) - A CoreDNS plugin to create records for Kubernetes nodes.
- [multicluster](https://github.com/coredns/multicluster/) - CoreDNS plugin implementing K8s multi-cluster services DNS spec.
- [ebpf](https://github.com/InfobloxOpen/ebpf) - A CoreDNS plugin that will attach an eBPF XDP program to a specified interface
- [rrl](https://github.com/coredns/rrl) - Response Rate Limiting Plugin for CoreDNS
- [mysql](https://coredns.io/explugins/mysql/) - MySQL backend for CoreDNS
- [warnlist](https://coredns.io/explugins/warnlist/) - emits logs and Prometheus metrics when a listed domain is requested.
- [git](https://github.com/miekg/coredns-git) - git middleware for Caddy
- [alternate](https://github.com/coredns/alternate) - Plugin Alternate is able to selectively forward the query to another upstream server, depending the error result provided by the initial resolver
- [k8s_dns_chaos](https://github.com/chaos-mesh/k8s_dns_chaos) - enables inject DNS chaos in a Kubernetes cluster for Chaos Engineering.
- [records](https://github.com/coredns/records) - A plugin that enables serving (basic) zone data directly from the Corefile
- [k8s_gateway](https://github.com/ori-edge/k8s_gateway) - A CoreDNS plugin to resolve all types of external Kubernetes resources
- [netbox](https://github.com/oz123/coredns-netbox-plugin/) - A coredns plugin to get dns records from Netbox
- [mdns](https://github.com/openshift/coredns-mdns) - CoreDNS plugin that serves .local mDNS info over normal DNS
- [wgsd](https://github.com/jwhited/wgsd) - A CoreDNS plugin that provides WireGuard peer information via DNS-SD semantics
- [alias](https://github.com/serverwentdown/alias) - CoreDNS plugin for replacing CNAME records on zone apex
- [fanout](https://github.com/networkservicemesh/fanout) - Repository for the coredns fanout plugin used by Network Service Mesh
- [lighthouse](https://github.com/submariner-io/lighthouse/tree/devel/coredns/plugin) - Controller to facilitate DNS discovery in multi-cluster environments
- [idetcd](https://github.com/jiachengxu/idetcd) - An etcd-based CoreDNS plugin used for identifying nodes in a cluster without domain name collisions.
- [gravwell](https://github.com/gravwell/coredns) - Gravwell CoreDNS plugin
- [amazondns](https://github.com/wadahiro/coredns-amazondns) - Amazon DNS plugin for CoreDNS
- [kubernetai](https://github.com/coredns/kubernetai) - Multiple Kubernetes in CoreDNS
- [redisc](https://github.com/miekg/redis) - CoreDNS plugin implementing a shared cache using Redis
- [unbound](https://github.com/coredns/unbound) - CoreDNS plugin that performs recursive queries using libunbound
- [on](https://github.com/coredns/caddy/tree/master/onevent) - executes a command when a specified event is triggered.
- [dump](https://github.com/miekg/dump) - dumps all incoming queries on standard output.
- [pdsql](https://github.com/wenerme/coredns-pdsql) - uses powerdns generic sql as backend.
- [ipin](https://github.com/wenerme/coredns-ipin) - CoreDNS plugin resolve the domain to ip in domain name
- [redis](https://github.com/arvancloud/redis) - redis plugin for coredns
- [demo](https://github.com/coredns/demo) - returns 1.1.1.1 for 172.0.0.0/8 or 127.0.0.0/8 and 8.8.8.8 otherwise
- [example](https://github.com/coredns/example) - prints ‘example’ on every query received.
- [ens](https://github.com/wealdtech/coredns-ens) - serve DNS records from the Ethereum Name Service.
- [ipecho](https://github.com/Eun/coredns-ipecho) - parses the IP out of a subdomain and echos it back as an record
- [blocklist](https://github.com/relekang/coredns-blocklist) - return NXDOMAIN response for any domain on preloaded lists. It can be useful to block malware domains or trackers.
- [ads](https://github.com/missdeer/ads) - DNS AdBlocker plugin for CoreDNS. :skull:
- [ipset](https://github.com/missdeer/ipset) - ipset plugin for CoreDNS
- [dnsredir](https://github.com/leiless/dnsredir) - Yet another seems better forward/proxy plugin for CoreDNS
- [bogus](https://github.com/missdeer/bogus) - return NXDOMAIN directly if the resovled IP is in the bogus list.
- [dockerdiscovery](https://github.com/kevinjqiu/coredns-dockerdiscovery) - Docker Discovery Plugin for CoreDNS
- [dogstatd](https://github.com/segmentio/coredns-plugins/tree/master/dogstatsd) - publish coredns metrics to dogstatsd agents
- [consul](https://github.com/segmentio/coredns-plugins/tree/master/consul) - DNS interface to consul with caching support


## Books

- [Learning CoreDNS](https://www.oreilly.com/library/view/learning-coredns/9781492047957/)


## Tutorials and Blog Posts

### CoreDNS inside K8s

- [A closer look at CoreDNS](https://medium.com/opstree-technology/a-closer-look-at-coredns-9968a1949577)
- [K8s - CoreDNS](https://blog.devgenius.io/k8s-dns-b798ea9db512)
- [Using CoreDNS effectively with Kubernetes](https://medium.com/infracloud-technologies/using-coredns-effectively-with-kubernetes-bd79b05768f7)
- [DNS caching gone wrong](https://qasim-sarfraz.medium.com/dns-caching-gone-wrong-a329dc00452e) - dnsmasq caching issues with CoreDNS
- [Using CoreDNS to Conceal Network Identities of Services in Istio](https://thecloudblog.net/post/using-coredns-to-conceal-network-identities-of-services-in-istio/)
- [CoreDNS and Route53](https://nicks-playground.net/posts/2019-11-26-coredns-and-route53/)
- [How to monitor CoreDNS](https://sysdig.es/blog/how-to-monitor-coredns/)
- [Kubernetes DNS for Services and Pods](https://medium.com/kubernetes-tutorials/kubernetes-dns-for-services-and-pods-664804211501)
- [Creating greater reliability: CoreDNS-nodecache](https://www.contentful.com/blog/coredns-nodecache-blog/) 
- [A Practical Guide to AWS Elastic Kubernetes Service Cross-Cluster Service Discovery using Consul](https://www.linkedin.com/pulse/practical-guide-aws-elastic-kubernetes-service-using-consul-rahul/)
- [K8s Troubleshooting — How to Debug CoreDNS Issues](https://medium.com/geekculture/k8s-troubleshooting-how-to-debug-coredns-issues-724e8b973cfc)
- [It’s not always DNS — unless it is](https://medium.com/adevinta-tech-blog/its-not-always-dns-unless-it-is-16858df17d3f)


### CoreDNS outside K8s

- [run your own nameservers with coredns](https://www.gophp.io/run-your-own-nameservers-with-coredns/)
- [Monitoring CoreDNS with Prometheus and New Relic](https://newrelic.com/blog/how-to-relic/monitor-coredns)
- [Setup a forwarding DNS Sinkhole with DNS over TLS&HTTPS](https://jmattheis.de/blog/setup-a-forwarding-dns-sinkhole-with-dns-over-tlshttps)
- [Coredns for local DNS resolution and forwarding over TLS (with Adblocking)](https://www.reddit.com/r/selfhosted/comments/jk9g61/coredns_for_local_dns_resolution_and_forwarding/)
- [CoreDNS: File Plugin for Lab Testing](https://cloudcult.dev/coredns-for-lab-testing/)
- [Setup a local devenv with CoreDNS, SSH and Docker Swarm](https://dklesev.github.io/devenv/)
- [CoreDNS on MacOS for local development](https://brendanthompson.com/posts/2021/12/coredns-on-macos-for-local-development)
- [Run Your Own Home DNS on coredns](https://blog.idempotent.ca/2018/04/18/run-your-own-home-dns-on-coredns/)
- [Serve using CoreDNS file plugin](https://savvythrough.medium.com/serve-using-coredns-file-plugin-23b4b1e20d96)
- [Serving dns in docker with coredns and consul agent](https://ilhicas.com/2023/01/25/Creating-a-core-dns-with-consul-docker-image.html)


## Videos

- [Intro to CoreDNS](https://www.youtube.com/watch?v=ZFEa2pDpvws) - Intro to CoreDNS by Miek Gieben (Creator of CoreDNS)
- [Understanding CoreDNS in Kubernetes](https://www.youtube.com/watch?v=qRiLmLACYSY) - An explanation of how CoreDNS works inside Kubernetes
- [Deep dive into CoreDNS](https://www.youtube.com/watch?v=rNlSgYZoIYs&) - Talk about CoreDNS at KubeCon Europe 2022
- [CoreDNS beyond the basics](https://www.youtube.com/watch?v=ym1uWYzxpEE) - KubeCon 2019
- [CoreDNS Intro And Deep Dive](https://www.youtube.com/watch?v=6TkrrZLxQeo) - KubeCon North America 2022
- [Introduction to CoreDNS](https://www.youtube.com/watch?v=um1ODpLrvsw) - Miek Gieben on the Rawkode Live Podcast
- [Building Custom CoreDNS Plugins](https://www.youtube.com/watch?v=ZffZzGbjy1k) - How to write your own CoreDNS plugin
- [Kubernetes DNS Horror Stories (And How to Avoid Them)](https://www.youtube.com/watch?v=Yq-SVNa_W5E) - Datadog on there experiences with CoreDNS on Kubernetes
- [Service Discovery with CoreDNS Plugins in Golang](https://www.youtube.com/watch?v=PtG0xlh5eSs) - KubeCon 2020 talk on creating a CoreDNS plugin
- [Service Discovery With Hybrid and Multi-Cloud](https://www.youtube.com/watch?v=vvVmx0EDdkw) - KubeCon 2019 talk on how to setup CoreDNS for Multi-Cloud
- [Lightning Talk: Is Your Kubernetes Cluster's DNS Working?](https://www.youtube.com/watch?v=thBCB7YeZ2g) - KubeCon 2019 talk on DNS troubleshooting
- [How DNS inside Kubernetes (CoreDNS) functions](https://www.youtube.com/watch?v=LBsZYPUUGuM) - Hand's on demo on the basic functioning of CoreDNS inside Microk8s, helping to resolve services and pods dns queries.


## Podcast Episodes

- [CoreDNS, with John Belamaric](https://open.spotify.com/episode/7jU6ggH7OY68NonBpJ8NUd?si=-DQfwhzwTFqabrC8Cd72IQ&nd=1)


## Tools

- [perf-test](https://github.com/coredns/perf-tests) - Scripts and utilities for scale and performance testing of CoreDNS.
- [deployment](https://github.com/coredns/deployment) - Scripts, utilities, and examples for deploying CoreDNS.
- [helm](https://github.com/coredns/helm) - Helm Charts for CoreDNS
- [corefile-migration](https://github.com/coredns/corefile-migration) - Library and tools for migrating the CoreDNS corefile
- [ansible](https://github.com/cloudalchemy/ansible-coredns) - Deploy CoreDNS using ansible.
- [charmed CoreDNS operator](https://github.com/charmed-kubernetes/charm-coredns) - CoreDNS operator for [Charmed Kubernetes](https://github.com/charmed-kubernetes)
