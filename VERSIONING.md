# ACE Protocol Versioning

The ACE Protocol uses **semantic versioning**:

- **MAJOR** – breaking changes to the ACE‑CERT structure  
- **MINOR** – new fields or non‑breaking additions  
- **PATCH** – clarifications or documentation updates  

Examples:

- `1.0.0` – initial stable release  
- `2.0.0` – structural change requiring new implementations  
- `1.1.0` – added optional field  
- `1.0.1` – documentation fix  

All versions of the protocol must remain publicly accessible.  
Implementations must declare which protocol version they support.
