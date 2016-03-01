# accouch-proxy

Proxy server that goes in front of CouchDB to add:

- Advanced authentication strategies, eg. third-party, multi-factor, better crypt
- Managable, inspectable, revocable, server-side stored sessions
- Database provisioning

## Setup

Set these environment variables:

- `COUCHDB_URL`: URL of CouchDB instance to use for storing user account info and provisioning databases. Needs server admin permissions.
- `REDIS_URL`: optional URL to use Redis for storing sessions, instead of CouchDB.
