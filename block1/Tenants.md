## Tapis Tenancy and Authorization

The Tapis authentication subsystem provides two mandatory components together with a set of optional services to enable institutions to integrate their existing identity providers and related systems. Tapis authentication is closely related to the notion of **tenancy** <br/>
A **tenant** in the Tapis framework represents a logical separation of Tapis entities (i.e., apps, jobs, actors, etc.) as well as a high-level authentication and security configuration. <br/>
Signed JSON Web Tokens represent the sole mechanism for proving identity to any Tapis API. As each tenant is configured with its own public key for token signatures, the entire authentication system can be customized on a per-tenant basis. 


[Tapis tenancy and authorization slides](https://docs.google.com/presentation/d/12RJSnEim0fhuSP2giu9y4ptBcOnsgpexjPL36LEalYI/edit?usp=sharing)