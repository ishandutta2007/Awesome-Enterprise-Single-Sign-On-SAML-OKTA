# Awesome-Enterprise-Single-Sign-On-SAML-OKTA

## Top Enterprise Single Sign-On (SAML/Okta) Ecosystem

**Curated List of SaaS Platforms & Open-Source GitHub Projects**  
*Focused on SAML Federation, OIDC Providers & Self-Hosted Identity Platforms*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Enterprise Single Sign-On (SAML/Okta)**. These tools help organizations centralize authentication across applications—covering everything from commercial IdP suites like Okta and Entra ID to open-source identity providers that speak SAML 2.0, OIDC, and OAuth 2.0 without per-user licensing.

**Examples** include Okta, Microsoft Entra ID, PingFederate, OneLogin, Auth0, Keycloak, Authentik, Casdoor, and ZITADEL (the category leaders).

**Open-source emphasis**: This section highlights every major active project for self-hosted SSO, open-source SAML/OIDC identity providers, and community-driven authentication platforms—ideal for organizations seeking data sovereignty and avoiding per-user SaaS pricing that compounds across workforces. The open-source landscape is genuinely mature: **Keycloak** is the CNCF-incubated standard with the deepest Java extension points , **Authentik** offers the most flexible sign-in flow engine , **Casdoor** provides a lightweight Go binary with built-in LDAP/RADIUS and MCP support , and **ZITADEL** delivers event-sourced audit trails with strict multi-tenancy .

Contributions welcome! Open an PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

| Product | Description | Pricing (Starting) | Free Tier / Trial Limits |
|---------|-------------|-------------------|--------------------------|
| **[Okta](https://www.okta.com/)** | **The enterprise SSO benchmark.** Workforce Identity supports SAML 2.0, OIDC, and OAuth 2.0 federation across thousands of pre-built app integrations. **Workforce Starter: $6/user/month** (annual); Enterprise: $17/user/month. | Starter: **$6/user/month**; Enterprise: **$17/user/month** | No free tier for workforce; developer edition available |
| **[Microsoft Entra ID](https://www.microsoft.com/en-us/security/business/identity-access/microsoft-entra-id)** | Cloud IAM with SAML 2.0 and OIDC federation, conditional access, and hybrid identity synchronization. **P1: $6/user/month**; P2: $9/user/month adds Identity Protection. | P1: **$6/user/month**; P2: **$9/user/month** | **Free edition**: basic SSO and security defaults with Azure/M365 subscriptions |
| **[PingFederate](https://www.pingidentity.com/)** | Enterprise federation server supporting SAML 2.0, OIDC, WS-Federation, and WS-Trust. Positioned for large organizations with complex federation requirements. **PingOne Workforce: from $3/user/month** (minimum 5,000 users). | Workforce: **$3/user/month** (min 5,000) | No free tier; demo via sales |
| **[OneLogin](https://www.onelogin.com/)** | Mid-market SSO with SAML and OIDC support. **Advanced tier: $4/user/month**; Professional: $8/user/month (verified 2026). | Advanced: **$4/user/month**; Professional: **$8/user/month** | Free trial available |
| **[Auth0](https://auth0.com/)** | Developer-first identity platform with SAML and OIDC support. **Free tier: ~25,000 MAU**; Essentials from $35/month. | Essentials: **$35/month** (up to 500 MAU) | **Free**: ~25,000 MAU, unlimited logins, no credit card |
| **[Google Workspace SSO](https://workspace.google.com/)** | SAML-based SSO within Google Workspace. Available on Business and Enterprise plans. | Business Starter: **$7/user/month** | **14-day free trial**; no permanent free tier |

## Open-Source GitHub Projects

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[Keycloak](https://github.com/keycloak/keycloak)** | [![Stars](https://img.shields.io/github/stars/keycloak/keycloak?style=social&color=white)](https://github.com/keycloak/keycloak/stargazers) | **The most widely deployed open-source SSO platform with proven enterprise scale.** Apache-2.0, Java/Quarkus. **SAML 2.0, OIDC, and OAuth 2.0** support with **realms for multi-tenancy**. **LDAP/Active Directory federation** and **SCIM 2.0 server support since 26.8**. **The most extension points for Java developers**—custom authentication flows via SPIs . **Trade-off**: JVM overhead and a build step when changing providers . **Best for enterprises needing battle-tested SSO** with deep Java customization and CNCF/Red Hat backing . |
| **[Authentik](https://github.com/goauthentik/authentik)** | [![Stars](https://img.shields.io/github/stars/goauthentik/authentik?style=social&color=white)](https://github.com/goauthentik/authentik/stargazers) | **The most flexible open-source sign-in flow engine.** MIT core with paid enterprise features. **Flows and stages** edited in the admin interface—custom authentication logic without code . **SAML 2.0, OIDC, OAuth 2.0, LDAP, RADIUS, and SCIM** support. **SCIM provider (push users to apps)**—a capability Keycloak and Casdoor lack . **Proxy provider** for Traefik, Caddy, Nginx, and Envoy . **Best for teams needing maximum sign-in flow flexibility** and SCIM provisioning to downstream apps . |
| **[Casdoor](https://github.com/casdoor/casdoor)** | [![Stars](https://img.shields.io/github/stars/casdoor/casdoor?style=social&color=white)](https://github.com/casdoor/casdoor/stargazers) | **Lightweight Go-based SSO with the widest protocol coverage.** Apache-2.0. **Single Go binary + React UI**—no JVM, no separate worker process. **SAML 2.0, OIDC, OAuth 2.0, CAS, LDAP, RADIUS, and SCIM** all supported. **Built-in MCP server with OAuth 2.1 for AI agents**—no other open-source IdP offers this natively . **70+ social/enterprise providers** including WeChat, DingTalk, and Lark. **Syncers import users from Keycloak, Okta, Entra ID, and Google Workspace**—enabling gradual migration . **Best for teams wanting a lighter, UI-first IdP** with legacy protocol support and AI-agent readiness . |
| **[ZITADEL](https://github.com/zitadel/zitadel)** | [![Stars](https://img.shields.io/github/stars/zitadel/zitadel?style=social&color=white)](https://github.com/zitadel/zitadel/stargazers) | **Event-sourced SSO with strict multi-tenancy and complete audit trails.** AGPL-3.0, Go/TypeScript. **SAML 2.0, OIDC, OAuth 2.0, and SCIM** support. **Instances → Organizations → Projects** hierarchy provides **infrastructure-level tenant isolation** . **Every mutation is an immutable event** for a complete, API-accessible audit trail—streamable to external systems via webhooks . **API-first design** with connectRPC, gRPC, and REST. **Best for organizations needing the strongest audit trail and tenant isolation** with a modern API-first design . |

### Additional Strong Open-Source Options

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[WSO2 Identity Server](https://github.com/wso2/product-is)** | [![Stars](https://img.shields.io/github/stars/wso2/product-is?style=social&color=white)](https://github.com/wso2/product-is/stargazers) | **Open-source IAM with SAML, OIDC, OAuth2, SCIM 2.0, and FIDO2 support.** Apache-2.0. Recognized as a Digital Public Good by the Digital Public Goods Alliance . **Used in 93 countries** across finance, public administration, healthcare, and telecommunications . **Best for organizations wanting a recognized open-source IAM** with broad standards support and enterprise adoption . |
| **[Janssen Project](https://github.com/JanssenProject/jans)** | [![Stars](https://img.shields.io/github/stars/JanssenProject/jans?style=social&color=white)](https://github.com/JanssenProject/jans/stargazers) | **Linux Foundation-governed IAM server providing OAuth 2.0, OIDC, SAML, FIDO2/WebAuthn, and SCIM.** Apache-2.0. **Kubernetes-native with auto-scaling** for enterprise and national scale . **Low-code flow orchestration (Agama) and policy engine (Cedarling)** for custom authentication logic without forking the core . **Best for organizations needing population-scale SSO** with strong federation readiness and Digital Public Good recognition . |
| **[Authelia](https://github.com/authelia/authelia)** | [![Stars](https://img.shields.io/github/stars/authelia/authelia?style=social&color=white)](https://github.com/authelia/authelia/stargazers) | **Lightweight authentication and authorization server with 2FA and SSO for web applications.** Go-based. Protects internal services behind a reverse proxy with minimal overhead . **Best for homelabs and small teams** needing SSO without a full IdP . |

**Frameworks for building custom systems**: Choose **Keycloak** for proven enterprise SSO with the broadest Java extension ecosystem , **Authentik** for the most flexible sign-in flows and SCIM provisioning , **Casdoor** for a lightweight Go binary with built-in LDAP/RADIUS and AI-agent MCP support , or **ZITADEL** for event-sourced audit trails and strict tenant isolation —all without per-user pricing that compounds across large workforces.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- SSO platforms handle authentication credentials and identity data; enforce MFA, least-privilege access, and compliance with applicable regulations (GDPR, SOC 2, HIPAA where relevant). **A compromised IdP exposes every connected application.**
- **Open-source SSO has four mature leaders with distinct trade-offs.** **Keycloak** is the most widely deployed with the deepest Java extension points, but requires JVM expertise and carries a build step for provider changes . **Authentik** has the **most flexible sign-in flow engine** and the only SCIM provider among the four, but its core is MIT with enterprise features under a commercial license . **Casdoor** is the lightest to run (single Go binary) and uniquely offers **built-in LDAP/RADIUS servers and MCP support for AI agents**, plus migration syncers from Keycloak/Okta/Entra ID, but has a smaller community than Keycloak . **ZITADEL** provides the strongest audit trail through event sourcing, but its AGPL-3.0 license may matter for some organizations . **Commercial platforms are quote-only at enterprise scale** except Okta ($6–$17/user/month), Entra ID ($6–$9/user/month), OneLogin ($4–$8/user/month), and Auth0 (free tier to 25K MAU) . **Validate protocol requirements (SAML, CAS, LDAP, RADIUS), multi-tenancy model, and operational capacity** before committing.

---

**Made for identity architects, IT administrators, and organizations building authentication infrastructure.**  
Let's make enterprise single sign-on more open, interoperable, and secure.
