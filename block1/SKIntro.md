## Distributed Security 

In our overview of Tapis security, we present the main components of a distributed security architecture and the authentication and authorization flows they support.  We describe how roles, permissions and secrets are managed and our plan for multisite implementations.  We also introduce our deployment strategy.<br/>

The Tapis security subsystem is comprised of four primary components, namely the **Tokens API**, **Authentication Server**, **Tenants API** and **Security Kernel**.  The Tokens API is a **stateless** mircoservice, which provides a reference implementation for generating a well-formatted, **signed JWT**. The Authentication server is **OAuth2** and **OIDC** complaint web server, which is capable of authenticating and generating signed JWT's using the Tokens service for end users. It is capable of integrating with an institution's **LDAP server**. The Tenant's API is used by system administrators to manage the registry of tenants distributed globally in a given Tapis installation, and by Tapis services for various operational tasks. These tenant specific properties, such as the public key that is used to sign JWTs, the locations of other Tapis services, etc., can be extracted from public endpoints provided by the API. <br/>

Lastly, the Security Kernel (SK) plays an important role in authentication and authorization; it is comprised of open-source software components tied together by a unifying API. SK builds upon the [Apache Shiro](https://shiro.apache.org) security framework to create a scalable, fine-grained authorization facility.  It extends the Shiro authorization model to allow permissions on hierarchical containers, such as file system directories, to extend to their subtrees. SK also incorporates the [Hashicorp Vault](https://www.vaultproject.io/) secrets store , which manages all secrets in the system, including all passwords and keys for databases, services and users. The security kernel API allows the platform's microservices to securely interact with users' storage and execution resources and with each other. <br/>

[Distributed Security Slides](https://docs.google.com/presentation/d/1BJOFLRjurYtaeAC7BoJIT6KqDPdFkkuuRuc7YptPvp4/edit?usp=sharing)



