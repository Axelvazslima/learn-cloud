# Global Networking

## Domain Name System (DNS)

Customers enter the web and browser a name to enter website -> it works because of DNS.

DNS resolution involves a customer DNS resolver communicating with a company DNS server.

```sh
DNS is the "phone book" of the internet and DNS resolution is the process of translating a domain name into an IP address.
```

Customer and PC --> Customer DNS resolver <--> (> What's the IP address for my wanted website? | < {IP Address}) Company DNS server

## Amazon Route 53

```sh
DNS web service. Reliable way of routing end users to applications hosted in the AWS cloud.
```

**Routing policies**
    * Latency-based routing
    * Geolocation DNS
    * Geoproximity routing
    * Weighted round robin

It routes users to infrastructure running in AWS (E.g. EC2 instances or load balancers). It can also route users to infrastructure out of the AWS environment.

Manages DNS records for domain names. Register new domains and tranfer domains -> Manage all your domains in a single place.

Client --> [Amazon Route 53, Amazon CloudFront --> Application Load Balancer --> [Auto scaling group [Amazon EC2 instances]]]

## Amazon CloudFront

Speedup delivery content from web sites to customers -> reduce latency.

Saving content as close to customers as possible -> CDN and edge locations.

