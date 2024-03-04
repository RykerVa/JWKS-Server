# JWKS-Server

This is a Go web server that provides a RESTful JWKS endpoint and an authentication endpoint for issuing JWTs. The JWKS endpoint serves public keys with unique identifiers (kid) for verifying JSON Web Tokens. Each key is associated with an expiry timestamp for enhanced security. The authentication endpoint returns unexpired, signed JWTs on a POST request. Additionally, if the "expired" query parameter is present, it issues a JWT signed with an expired key pair and expiry.
