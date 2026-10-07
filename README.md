# Awesome-Cloud-Service-Discovery

# Awesome-Cloud-Service-Discovery 🔍 ☁️



<p align="center">

  <img src="assets/banner.svg" alt="Awesome Cloud Service Discovery Banner" width="100%">

</p>



<p align="center">

  <a href="https://github.com/ishandutta2007/Awesome-Awesome-Awesome"><img src="https://img.shields.io/badge/Awesome-%E2%9C%94-blueviolet?style=flat-square&logo=github" alt="Awesome"/></a>

  <a href="https://discord.gg/jc4xtF58Ve"><img src="https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="Discord" /></a>

  <a href="https://github.com/ishandutta2007/Awesome-Cloud-Service-Discovery"><img src="https://img.shields.io/github/stars/ishandutta2007/Awesome-Cloud-Service-Discovery?style=social" alt="GitHub_Stars"/></a>

  <a href="https://github.com/ishandutta2007/Awesome-Cloud-Service-Discovery/fork"><img src="https://img.shields.io/github/forks/ishandutta2007/Awesome-Cloud-Service-Discovery?style=social" alt="GitHub Forks"/></a>

  <a href="https://github.com/ishandutta2007/Awesome-Cloud-Service-Discovery/blob/main/LICENSE"><img src="https://img.shields.io/github/license/ishandutta2007/Awesome-Cloud-Service-Discovery?color=blue" alt="License"/></a>

  <a href="https://github.com/ishandutta2007"><img alt="GitHub followers" src="https://img.shields.io/github/followers/ishandutta2007?label=Follow" /></a>

</p>



---



## 🌟 Top Cloud Service Discovery Ecosystem



**Curated List of Commercial Service Discovery Platforms & Open-Source Service Registry Tools**  

*Focused on DNS-Based Discovery, Key-Value Registries, Service Mesh Integration, Health Checking & Self-Hosted Service Catalogs*



**Last updated: October 2026** 📅



---



### 📌 Overview & SEO Summary

Welcome to the ultimate curated directory of **cloud service discovery platforms**, **open-source service registry tools**, and **DNS-based discovery frameworks**. Whether you are looking for enterprise-grade commercial solutions (such as *AWS Cloud Map*, *HashiCorp Consul*, and *Netflix Eureka*), or self-hostable open-source alternatives (like *CoreDNS*, *etcd*, and *ZooKeeper*), this list covers category leaders, service mesh integration, and privacy-respecting service registries.



---



## 📑 Table of Contents

- [🏢 SaaS & Commercial Platforms](#-saas--commercial-platforms)

- [🔓 Open-Source GitHub Projects](#-open-source-github-projects)

- [🛠️ How to Contribute](#%EF%B8%8F-how-to-contribute)

- [📊 Star History](#-star-history)

- [🤝 Support & Sponsorship](#-support--sponsorship)

- [⚠️ Disclaimer](#%EF%B8%8F-disclaimer)



---



## 🏢 SaaS / Commercial Platforms



The service discovery market spans **cloud provider native services** (AWS Cloud Map) that provide fully managed service registries integrated with cloud infrastructure, **service mesh control planes** (Istio, Linkerd, Traefik Mesh) that embed discovery into their data planes, and **standalone service registries** (Consul, Eureka, ZooKeeper) that serve as dedicated discovery infrastructure.



| SaaS / Commercial Platform | Company / Owner | Valuation / Market Cap | Standard Edition Starting Price | Free Tier / Free Trial Limits | Description |

| :--- | :--- | :--- | :--- | :--- | :--- |

| **[AWS Cloud Map](https://aws.amazon.com/cloud-map/)** ☁️ | Amazon | ~$2.0 Trillion | **Pay-as-you-go** per resource and API call  | **No upfront costs**; pay only for usage  | **AWS-native service discovery** — Maps logical names to backend services and resources. Uses **DiscoverInstances API** or **DNS queries** for discovery . Returns only healthy resources. Integrates with Route 53 health checks . |

| **[HashiCorp Consul](https://www.consul.io/)** 🔐 | HashiCorp (IBM) | ~$5 Billion (Acquisition) | **Community: Free**; **Enterprise: Custom** | **Community Edition free forever** | **Multi-runtime service discovery** — **Consul DNS** enables application load balancing and static service lookups . **Prepared queries** for dynamic lookups and service failover across datacenters . Raft consensus for high availability. Integrates with NGINX and HAProxy . |

| **[Netflix Eureka](https://github.com/Netflix/eureka)** 🎬 | Netflix OSS | N/A (Open Source) | **Free** | **Open-source free forever** | **REST-based service discovery** — Netflix's battle-tested service registry for its vast microservice ecosystem . **Client-server model**: services register and send periodic heartbeats. **Port 8761** commonly used . Java-based, part of Netflix OSS. |

| **[Istio Service Registry](https://istio.io/)** 🔷 | Istio (Google/IBM/Lyft) | N/A (Open Source) | **Free** | **Open-source free forever** | **Service mesh with embedded discovery** — **ServiceEntry** registers external services in Istio's mesh registry . Provides service-level telemetry, traffic policies, and TLS origination for external calls . Integrated with Kubernetes service discovery. |

| **[Traefik Mesh](https://traefik.io/)** 🚦 | Traefik Labs | Private | **Free** (open-source core) | **Open-source free forever** | **Lightweight service mesh** — Automatic service discovery via **labels and metadata** . **mTLS encryption** by default. Discovers new instances through labels — no config reloads . Routes internal traffic with identity baked in . |

| **[Linkerd](https://linkerd.io/)** 🦊 | Buoyant | Private | **Free** (open-source) | **Open-source free forever** | **Ultralight service mesh** — For Kubernetes services, looks up IPs via **Kubernetes API** and load balances across endpoints . For non-Kubernetes destinations, balances across **DNS-provided endpoints** . |



---



## 🔓 Open-Source GitHub Projects



*Sorted by GitHub_Stars_Count (Descending)* 🌟



- **[CoreDNS](https://github.com/coredns/coredns)** [![Stars](https://img.shields.io/github/stars/coredns/coredns?style=social&color=white)](https://github.com/coredns/coredns/stargazers)  

  **DNS server and service discovery framework**, Apache-2.0 licensed. **Written in Go** for flexibility and performance . **Chains plugins** — each plugin performs a DNS function like Kubernetes service discovery, Prometheus metrics, or zone file serving . **Integrates with Kubernetes** via the Kubernetes plugin, with **etcd** via the etcd plugin, and with **all major cloud providers** (Azure DNS, GCP Cloud DNS, AWS Route53) . **Compile with only the plugins you need** for minimal footprint. **The de facto standard for Kubernetes DNS-based service discovery** — used by OpenShift's DNS Operator to provide name resolution for pods . 🎯



- **[etcd](https://github.com/etcd-io/etcd)** [![Stars](https://img.shields.io/github/stars/etcd-io/etcd?style=social&color=white)](https://github.com/etcd-io/etcd/stargazers)  

  **Distributed reliable key-value store for the most critical data of a distributed system**, Apache-2.0 licensed. **The foundational coordination service for Kubernetes** — stores all cluster state . **Service discovery via leases and watchers** — services register with a TTL lease, and clients watch for changes . **CoreDNS etcd plugin** implements SkyDNS service discovery from etcd . **Used by CoreDNS for SkyDNS-compatible discovery** . **The most widely deployed distributed key-value store for service discovery in cloud-native environments**. 🔑



- **[Apache ZooKeeper](https://github.com/apache/zookeeper)** [![Stars](https://img.shields.io/github/stars/apache/zookeeper?style=social&color=white)](https://github.com/apache/zookeeper/stargazers)  

  **Distributed coordination service**, Apache-2.0 licensed. **Service discovery via ephemeral nodes** — servers register on startup, and ZooKeeper automatically removes nodes when servers shutdown or crash . **Two discovery modes**: **Watch** (notifies clients immediately on changes) and **Poll** (periodic reads for large client counts) . **Apache Helix** provides higher-level abstraction with state machines, constraints, and dynamic configuration management . **The original distributed coordination service** — powers Kafka, HBase, and countless other systems. 🐘



- **[Apache Helix](https://github.com/apache/helix)** [![Stars](https://img.shields.io/github/stars/apache/helix?style=social&color=white)](https://github.com/apache/helix/stargazers)  

  **Cluster management framework for partitioned and replicated distributed resources**, Apache-2.0 licensed. **Service discovery built on ZooKeeper** with higher-level abstractions . **Automatically detects flapping** (repeated connect/disconnect) and disables bad nodes. **Dynamic configuration management** — change configuration without server restarts . **Disable nodes via admin API** without killing them (preserves debugging capability) . **The most sophisticated open-source service discovery framework** for complex distributed systems. 🎛️



- **[SkyDNS](https://github.com/skynetservices/skydns)** [![Stars](https://img.shields.io/github/stars/skynetservices/skydns?style=social&color=white)](https://github.com/skynetservices/skydns/stargazers)  

  **DNS service discovery from etcd**, MIT licensed. **The original etcd-based service discovery implementation** — CoreDNS's etcd plugin implements SkyDNS service discovery . **Encodes service data in etcd as SkyDNS message format** . **The foundational pattern for etcd-based service discovery** — inspired countless implementations. 📡



- **[Eureka (Netflix OSS)](https://github.com/Netflix/eureka)** [![Stars](https://img.shields.io/github/stars/Netflix/eureka?style=social&color=white)](https://github.com/Netflix/eureka/stargazers)  

  **REST-based service discovery server**, Apache-2.0 licensed. **Part of Netflix OSS** — battle-tested at Netflix's scale . **Client-server model** with registration, heartbeat, and discovery . **Clustering support** for high availability — registry replicated across all instances . **Java-based** with client libraries for multiple languages. **The most widely adopted Java service registry** — used by Spring Cloud Netflix. 🌐



---



## 🛠️ How to Contribute



Contributions are welcome! Follow these steps to submit new service discovery platforms or open-source registry software:



1. 🍴 **Fork** the repository.

2. 📝 **Add/edit** entries in `README.md` maintaining table/list structure and formatting.

3. 🔗 Include project title, official website/GitHub link, exact Stars_Count, license, and brief description.

4. 🚀 Submit a **Pull Request** with a descriptive summary of your changes.



---



## 📊 Star History



[![Star History Chart](https://star-history.dera.page/svg?repos=ishandutta2007/Awesome-Cloud-Service-Discovery&type=date&legend=top-left)](https://star-history.dera.page/#ishandutta2007/Awesome-Cloud-Service-Discovery&type=date&legend=top-left)



---



## 🤝 Support & Sponsorship



If you find this cloud service discovery repository useful, please consider supporting the project:



- ⭐ **Star** this repository to increase visibility!

- 🔀 **Fork** and share with fellow cloud architects, platform engineers, and open-source advocates.

- ☕ **Sponsor & Buy Me a Coffee**: Support ongoing open-source curation via the [GitHub Sponsor Dashboard](https://github.com/sponsors/ishandutta2007).



---



## ⚠️ Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement. ℹ️

- **AWS Cloud Map pricing is pay-as-you-go** based on registered resources and API calls — **Route 53 DNS and health checks incur additional charges** .

- **Consul DNS and service discovery are enabled by default** — when service mesh is enabled, you can use **CoreDNS with transparent proxy** .

- **ZooKeeper session expiry causes loss of watches and ephemeral nodes** — servers must detect flapping and deregister . **Watch mode can trigger herd effect** with hundreds of clients — use **Poll mode** for large client counts .

- **Open-source tools (CoreDNS, etcd, ZooKeeper) are not turnkey** — they require **deployment, integration, and ongoing maintenance**. **Always validate service discovery with a proof-of-concept** before production deployment. 🔍



---



<p align="center">

  <b>Made with ❤️ for cloud architects, platform engineers, and open-source service discovery advocates.</b>

</p>
