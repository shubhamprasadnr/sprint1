#  DNS Documentation 
![image](https://github.com/user-attachments/assets/de305691-3ca3-4f71-ad8e-3ac09b0b9472)

| Author  | Created on | Version   | Last Edited On | Comment  | Reviewer |
|---------|------------|-----------|----------------|-------------------|---------------|
| Shubham | 29-04-25   |  version1.1 | 01-05-25        | Internal Review    | Komal Jaiswal|


## Table of Contents
- [1. Introduction](#introduction)
- [2. What is DNS](#what-is-dns)
- [3. Why DNS is Needed](#why-dns-is-needed)
- [4. How DNS Works (Step-by-Step)](#how-dns-works-step-by-step)
- [5. How to Get a Domain](#how-to-get-a-domain)
- [6. Different DNS Providers](#different-dns-providers)
- [7. Detailed Comparison](#detailed-comparison)
- [8. Recommendation](#recommendation)
- [9. Contact ](#contact)
- [10. References](#references)

---


## Introduction

In this document, we will explain what DNS (Domain Name System) is, how it functions like the internet’s phonebook, and how multiple DNS servers work together to resolve domain names into IP addresses. We’ll also walk through the step-by-step process of how DNS works, and why it's a critical component in connecting users to websites and online services.

---

## What is DNS

The Domain Name System (DNS) is a hierarchical and decentralized naming system used to resolve human-readable domain names (like example.com) into machine-readable IP addresses (like 192.0.2.1). This system enables users to access websites and services using familiar names instead of numeric IP addresses.


## Why DNS?
| Reason                          | Description |
|---------------------------------|-------------|
| **Human-Friendly Navigation**   | Humans remember names better than numbers. DNS allows websites to have easy-to-remember names. |
| **Network Efficiency**          | DNS enables a distributed database that is highly scalable and efficient. |
| **Redundancy and Load Balancing** | DNS can distribute traffic among multiple servers to prevent overload. |
| **Security Enhancements**       | Modern DNS includes features like DNSSEC to secure domain data from attacks like cache poisoning. |


---



## How DNS Works (Step-by-Step)

When you type `www.example.com` into your browser:

| Step | Description |
|------|-------------|
| 1. **Browser Cache** | Checks if it already knows the IP from memory. |
| 2. **OS Cache** | If not found, asks your operating system's DNS cache. |
| 3. **Recursive Resolver** | If still not found, the query is sent to a DNS resolver (provided by your ISP or a public one like Google 8.8.8.8). |
| 4. **Root Server** | The resolver asks a Root Server where `.com` domains are managed. |
| 5. **TLD Server** | The resolver is directed to the `.com` TLD server. |
| 6. **Authoritative Server** | Finally, the resolver asks the authoritative server for `example.com`, which returns the IP address. |
| 7. **Website Loading** | Now, the browser uses the IP to establish a connection with the website server. |

📍 All this happens in milliseconds!
![image](https://github.com/user-attachments/assets/138a3160-5610-4503-86a9-0f864838a785)


---

## How to Get a Domain

Getting your own domain involves these simple steps:

| Step | Description |
|------|-------------|
| **1. Choose a Domain Name** | Pick a unique and relevant name for your brand or website. |
| **2. Find a Registrar** | Use a certified domain registrar like GoDaddy, Namecheap, or Google Domains. |
| **3. Check Availability** | Use the registrar’s search tool to ensure your desired name isn’t already taken. |
| **4. Purchase the Domain** | Register and pay for the domain, typically on a yearly basis. |
| **5. Set Up DNS Records** | Configure A, CNAME, MX, and other DNS records to point your domain to your web server or services. |




---

## Different DNS Providers

Some of the most popular DNS providers:

| Provider          | Services                              |
|-------------------|---------------------------------------|
| Cloudflare        | DNS, CDN, Security, DDoS protection   |
| Google DNS        | Public DNS resolver (8.8.8.8)         |
| Amazon Route 53   | Scalable DNS service, traffic routing |
| GoDaddy           | DNS with domain registration          |
| Namecheap         | Affordable domain + DNS management    |
| Dyn (Oracle)      | Managed DNS solutions                 |
| Akamai Edge DNS   | Enterprise-grade DNS performance      |

---

## Detailed Comparison

| Feature           | Cloudflare        | Google Public DNS | Route 53 (AWS)   | GoDaddy           | Namecheap        |
|-------------------|-------------------|-------------------|------------------|-------------------|------------------|
| **Speed**         | Very Fast          | Very Fast          | Fast             | Good              | Good             |
| **Ease of Use**   | Very Easy          | Very Easy          | Moderate         | Easy              | Very Easy        |
| **DDoS Protection** | Yes               | No                | Optional         | Basic             | Basic            |
| **Cost**          | Free (basic DNS)   | Free (resolver)    | Pay-as-you-go    | Paid (with domain) | Paid (with domain)|
| **Advanced Features** | CDN, WAF, SSL   | None              | Geo-routing, health checks | Basic | Basic |
| **Security (DNSSEC)** | Yes             | No                | Yes              | Yes               | Yes              |

➡️ **Summary**:  
- **Cloudflare** is best for free + secure DNS.
- **Route 53** is best for enterprises needing full cloud integration.
- **Google DNS** is good for individuals needing a reliable resolver.
- **GoDaddy/Namecheap** are good choices for simple domain purchases.

---

## Recommendation

| Situation                     | Recommendation        |
|--------------------------------|------------------------|
| **Startup / business website**| AWS Route 53 + Cloudflare |



---

## Contact 
| Name | Email Address |
|------|---------------|
| Shubham Prasad | [shubham.prasad.snaatak@mygurukulam.co](mailto:shubham.prasad.snaatak@mygurukulam.co) |



## References

| Links | Descriptions |
|-------|--------------|
| [AWS Rote53](https://k21academy.com/amazon-web-services/aws-solutions-architect/aws-route-53/) | Detailed Documentation OF Uses and Setup |

---
