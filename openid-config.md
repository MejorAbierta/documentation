# Official openID ✅

[Repo Official openID](https://github.com/pkp/openid) 
- Developer: PKP 
- Ver: OJS 3.4.0
- Protocol: openID
- Last update: Dec 12, 2024 
- Data: (RS256) JWT : 
```php
  {
   	'id' => $jwtPayload->sub ?? null,
  	'email' => $jwtPayload->email ?? null,
  	'username' => $jwtPayload->preferred_username ?? null,
  	'given_name' => $jwtPayload->given_name ?? null,
  	'family_name' => $jwtPayload->family_name ?? null,
  	'email_verified' => $jwtPayload->email_verified ?? null,
  }
  ```
- Review: Working
- Tested Ver : OJS 3.4 - stable, OJS 3.3, OMP 
- PKCE: No
- OJS config :
  - URL: example.com/.well-known/openid-configuration
  - ClientID
  - Secret
- Endpoint Config:
  - Signature Algorimth : RS256
  - Authentication Type: Authentication Code Flow
  - PKCE enabled : No
  - OJS URL

## CONFIG ORCID OPENID
- Go to https://orcid.org/developer-tools, sign in and configure URL and name of our service.
  Notes:
> **Only HTTPS** URIs are accepted in production
> Domains registered MUST exactly match the domains used, including subdomains
> Register all redirect URIs fully where possible. This is the most secure option and what we recommend.
> The ORCID Public **API is free for non-commercial use by individuals** as stated in the [Public APIs Terms of Service](https://info.orcid.org/public-client-terms-of-service/).
> ORCID's current Rate Limit is 24 requests per second for the Member, Public, and Anonymous APIs

## CONFIG Rediris OPENID
**Rediris** has an OpenID implementation:
[How to implement OpenId with Rediris](https://www.rediris.es/sir/howto-openid.html)
For use rediris is needed sign up here getting in touch with the organization https://www.rediris.es/sir/contacto.html.
