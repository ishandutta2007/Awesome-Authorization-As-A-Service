# Awesome-Authorization-As-A-Service

## Top Authorization-as-a-Service Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Fine-Grained Authorization, ReBAC/Zanzibar, Policy Decision Points, Externalized Permissions & AuthZ for Apps and Agents*  

**Last updated: September 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Authorization-as-a-Service**. These systems externalize access-control decisions—RBAC, ABAC, and relationship-based (ReBAC/Zanzibar)—so permissions stay consistent, auditable, and changeable without redeploying every service.



**Examples** include Permit.io, Cerbos, Aserto, AuthZed, Oso, OpenFGA, Topaz, PlainID, Styra DAS, and Axiomatics (the category leaders).



**Open-source emphasis**: Authorization has outstanding open engines. **OpenFGA**, **SpiceDB**, **Cerbos**, **Oso**, **Casbin**, **OPA**, and **Ory Keto** are production-proven. This section is heavily expanded.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[AuthZed (SpiceDB Cloud), OpenFGA Cloud-adjacent](https://authzed.com/)**  

  Managed Zanzibar-style permission databases—relationship tuples at scale with strong consistency options.



- **[Cerbos Hub, Permit.io, Aserto, Oso Cloud](https://www.cerbos.dev/)**  

  Policy-as-code and developer-friendly authorization platforms with hosted PDPs, policy hubs, and SDKs (open engines underneath).



- **[PlainID, Axiomatics, Styra DAS](https://www.plainid.com/)**  

  Enterprise authorization and policy platforms—central policy administration, ABAC, and large-scale decision services.



- **[Topaz & hybrid open/commercial offerings](https://www.topaz.sh/)**  

  Authorization products combining open policy engines with managed control planes.



- **[Other commercial AuthZ platforms](https://authzed.com/)**  

  Additional fine-grained authorization and entitlement management solutions.



## Open-Source GitHub Projects



- **[OpenFGA](https://github.com/openfga/openfga)**  

  CNCF open-source (Apache 2.0) authorization engine inspired by Google Zanzibar—ReBAC + ABAC, high performance, widely adopted.



- **[SpiceDB](https://github.com/authzed/spicedb)**  

  Open-source Zanzibar-inspired permissions database from AuthZed—schema + relationships with strong consistency focus.



- **[Cerbos](https://github.com/cerbos/cerbos)**  

  Open-source policy decision point—stateless, YAML/JSON policies, AuthZEN-friendly, embed or sidecar deployment.



- **[Oso](https://github.com/osohq/oso)**  

  Open-source authorization library with Polar policy language—embed policies next to application code (cloud product available).



- **[Casbin](https://github.com/casbin/casbin)**  

  Embeddable open authorization library—ACL/RBAC/ABAC models across many languages via CONF policy files.



- **[Open Policy Agent (OPA)](https://github.com/open-policy-agent/opa)**  

  General-purpose open policy engine (Rego)—widely used for AuthZ, admission control, and infrastructure policy.



- **[Ory Keto](https://github.com/ory/keto)**  

  Open-source permission system in the Ory stack—Zanzibar-style relationships integrated with identity products.



- **[Cedar (Amazon)](https://github.com/cedar-policy/cedar)**  

  Open policy language and SDK for deterministic, auditable authorization policies.



### Additional Strong Open-Source Options



- **Zanzibar/ReBAC**: OpenFGA or SpiceDB as the relationship store.

- **Policy-as-code PDP**: Cerbos or OPA for ABAC-style rules.

- **In-process**: Oso or Casbin when a library is preferred over a service.

- **Composable stacks**: Identity (Keycloak/Ory) → OpenFGA/SpiceDB or Cerbos → app enforcement.

- Commercial platforms still lead in policy UX, multi-tenant control planes, and enterprise support.



**Frameworks for building custom systems**:  

**OpenFGA** / **SpiceDB** for relationship-based AuthZ; **Cerbos** / **OPA** for policy-as-code; **Oso** / **Casbin** for embedded checks.  

Commercial AuthZ-as-a-Service (Permit.io, Cerbos Hub, AuthZed, Aserto, PlainID, etc.) adds managed scale and policy administration.  

Most modern apps can start fully open; adopt commercial control planes when policy teams need central governance. Fully open authorization is production-ready at significant scale.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Incorrect authorization can expose data or block legitimate users. Test policies thoroughly, log decisions, and apply least privilege. Relationship and attribute models must stay consistent with your identity source of truth.

- Open-source engines offer full control but require you to operate stores and policy pipelines. Commercial platforms shift operational burden to the vendor. Neither replaces careful design of roles, relationships, and resource hierarchies.



---



**Made for platform engineers, security architects, and teams externalizing permissions the right way.**  

Let's expand open, standards-based authorization while recognizing the policy UX and scale that leading commercial AuthZ platforms deliver.
