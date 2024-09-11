| **Feature**                                   | **Kerberos Version 5**               | **SAML 2.0**                           | **OpenID 2.0**                      | **OpenID Connect 1.0 (OIDC)**       | **OAuth 2.0**                       |
|-----------------------------------------------|--------------------------------------|----------------------------------------|-------------------------------------|-------------------------------------|-------------------------------------|
| **Purpose**                                   | Authentication protocol              | Authentication and authorization       | Decentralized authentication        | Authentication protocol built on OAuth | Authorization delegation protocol  |
| **Primary Use Case**                          | Network authentication within a domain | Web-based SSO                         | User authentication for websites    | Authentication and user identity    | Access delegation without sharing credentials |
| **Authentication Method**                     | Ticket-based                          | XML-based authentication assertions    | URL-based identity verification     | JSON Web Token (JWT) based           | Token-based                         |
| **Identification**                            | User principal name (UPN)             | NameID in SAML Assertion               | OpenID Identifier (URI)             | Sub claim in ID Token (JWT)          | Not applicable                      |
| **Identity**                                  | Managed within a domain (e.g., AD)    | Federated identity, managed across domains | User-centric, managed by provider  | User-centric, managed by provider    | Delegated through OAuth scopes      |
| **Authentication**                            | Yes                                   | Yes                                    | Yes                                 | Yes                                 | No                                  |
| **Authorization**                             | No                                    | Yes                                    | No                                  | Yes                                 | Yes                                 |
| **Token Type**                                | Ticket (TGT, ST)                      | SAML Assertion                         | Identifier URI                      | ID Token (JWT)                       | Access Token (JWT or others)        |
| **Single Sign-On (SSO)**                      | Yes                                   | Yes                                    | Yes                                 | Yes                                 | No                                  |
| **Multi-Factor Support**                      | Yes                                   | Yes                                    | No                                  | Yes                                 | No                                  |
| **Decentralized Identity**                    | No                                    | No                                     | Yes                                 | Yes                                 | No                                  |
| **Trust Model**                               | Centralized (within a domain)         | Federated (trust agreements)           | Decentralized                       | Decentralized                        | Delegated trust to resource owners  |
| **Interoperability**                          | Low (specific to Kerberos environments) | High                                  | Moderate                            | High                                 | High                                 |
| **Standards**                                 | RFC 4120                              | OASIS Standard                         | OpenID Foundation                   | OpenID Foundation                    | IETF                                 |
| **Typical Implementation**                    | Windows Active Directory, Unix        | Web applications, cloud services       | Web and mobile applications         | Web and mobile applications          | APIs, web, and mobile applications  |
| **Main Advantage**                            | Strong security within a domain       | Secure, standardized SSO               | User control over identity          | Modern, secure identity management   | Granular access control              |
| **Main Limitation**                           | Limited to specific environments      | Can be complex to implement            | Limited features                    | Requires OAuth as a foundation       | Focused on authorization, not authentication |
