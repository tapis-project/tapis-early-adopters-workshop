## Security Kernel

In our overview of Tapis security, we present the main components of a distributed security architecture and the authentication and authorization flows they support.  <br/>

The Tapis Security Kernel plays an important role in the authentication and authorization process and is a distributed subsystem comprised of open-source software components tied together by a unifying API. The Tapis Security Kernel builds upon [Apache Shiro](https://shiro.apache.org) security framework to create a scalable, fine-grained authorization facility by extending its permissions model with representations of file path names. It has a secrets store, [Hashicorp Vault](https://www.vaultproject.io/), which manages all secrets in the system, including all passwords and keys, using a fault-tolerant, scalable, highly available cluster of VMs. The security kernel provides an API that the platform's other microservices use to securely interact with users' storage and execution resources and with each other. 

We describe how roles, permissions and secrets are managed and our plan for multisite implementations. We also introduce our deployment strategy.

[Distributed Security](https://docs.google.com/presentation/d/1BJOFLRjurYtaeAC7BoJIT6KqDPdFkkuuRuc7YptPvp4/edit?usp=sharing)
