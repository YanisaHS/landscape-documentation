(reference-whats-new-in-beta)=
# What's new in beta

Here's what's new in Landscape beta:

## Landscape Server

landscape-server 25.04~beta.11 published 24 March 2025

  * refactor: revert message handler perfs
  * feat: add employee-access OIDC authentication API
  * feat: add script profile execute endpoint
  * feat: include employee_id in computer serialization
  * feat: create Google Workspace directory import module
  * feat: add import directory API endpoints
  * feat: add features supporting employee authorization
  * feat: add ability to manage script profiles
  * feat: add management class for autoinstall files
  * feat: add script profile limits endpoint

landscape-server 25.04~beta.10 unpublished

  * perf: improve processor info message handling
  * fix: download receipts in legacy UI
  * feat: implement database-backed secrets client
  * feat: add with_versions to autoinstall GET handler
  * feat: add provider details to oidc issuer handlers
  * feat: add filter and search to employees GET handler
  * fix: permission errors replaced with blank elements in new web portal
  * feat: add search and filter to autoinstall list handler
  * feat: add list_secret_metadata to secrets clients
  * feat: add script profile table
  * feat: alter autoinstall file reference in employee group table
  * fix: update the mirror lists
  * feat: add search and filter to employee group list handler
  * feat: add google service account model
  * feat: allow duplicate and null priorities in employee group table
  * feat: introduce script profiles
  * feat: process authenticated attach code in client registration messages
  * fix: allow employee, employee group, and autoinstall filters to take multiple ids
  * feat: add script profile run table
  * fix: make oidc issuer provider a property
  * fix: handle null fields in employee group
  * feat: add security endpoint
  * fix: bug in optimized free space message handler
  * feat: create JWT models for administrators and employees
  * feat: add authentication configurations to oidc issuer endpoints

landscape-server 25.04~beta.9 unpublished

  * feat: add list OIDC configurations endpoint
  * refactor: change PAYG forms to use Stripe forms instead
  * feat: add DirectoryAPI interface
  * feat: add bulk update/delete for employee groups
  * feat!: add secrets client stubs
  * feat: add autoinstall file model
  * feat: USG activity info class
  * feat: add configure and validation methods for autoinstall files
  * refactor: move common archived computer check to superclass
  * perf: improve handling of computer info messages

landscape-server 25.04~beta.8 published 24 February 2025

* feat: add query parameters to employee and employee_group GET/LIST endpoints
* perf: improve message api handling times
* feat: add id to autoinstall responses
* feat: add Ubuntu installer attach session model
* feat: add endpoint for deleting wsl child instances

landscape-server 25.04~beta.7 published 14 February 2025

* fix: make running profiles independent of updating/processing alerts
* feat: add archive endpoint
* fix: client reported package installed sizes larger than BIGINT
* feat: use OIDCAuthnConfiguration for OIDC endpoints
* fix: remove standalone provider from supported providers response
* fix: make logfile create perms CIS-compliant; proper signal to rsyslogd (LP: #2095406)
* feat: add CRUD endpoints for OIDC issuers
* feat: Implement employee management API stubs
* feat: Create database table for WSL instance names
* feat: remove account id from employee and employee_group model
* feat: refactor employee management API stubs to use issuer_id
* fix: make use of md5 hash FIPS compliant
* feat: add Google OAuth 2.0 to supported OIDC providers
* fix: bug in v2 api eventlog endpoint (LP: #2098367)
* fix: change access group api bug (LP: #2098365)
* feat: add OIDC group import model

landscape-server 25.04~beta.6 published 31 January 2025

* fix: log and handle non-JSON errors when querying package-search
* fix: remove the obsolete file README.multiple-services, plus references to it
* fix: reset passphrase oops
* fix: add ipv6 to pingserver
* feat: include has_password field in /me and /login responses
* feat: Add per-account custom OIDC configuration limit
* fix: ignore whitespace around annotation delimiter when searching for computers
* feat: add script profile limit table
* feat: add oidc_issuer and oidc_authn_configuration models
* fix: API call hangs when request path includes an extra slash
* feat: remove OIDC schema flexibility
* feat: add database tables for employees

landscape-server 25.04~beta.5 published 17 January 2025

* feat: add sanitize endpoint
* feat: create a sync activity for newly registered child instances
* fix: issue with pro free licenses
* fix: don't create whole transactions just to check if db conn is alive
* fix: script bug with carriage return characters in interpreter
* feat: added esm packages to hashid database file

landscape-server 25.04~beta.4 published 13 December 2024

* fix: username bug in legacy API endpoint to execute a script
* fix: schema migration bug in setup-landscape-server script
* fix: api test permissions
* feat: added changes to support invalidating jwt tokens
* fix: raise AuthenticationFailure for cookies that fail to decrypt
* feat: database models related to USG Profiles
* fix: 500 error in secrets list view in legacy UI
* fix: restore database connection in Storm stores if dropped

landscape-server 25.04~beta.3 published 29 November 2024
  * fix: bug preventing account switching in new UI
  * fix: configure a randomly-generated default `cookie-encryption-key` during
    startup if not provided
  * fix: redirect security to untrusted

landscape-server 25.04~beta.2 published 19 November 2024
  * fix: address inconsistent Account object updates on subdomain-aware
    API endpoints

landscape-server 25.04~beta.1 published 15 November 2024
  * feat: grpc server sends the request_id parameter
  * feat: standalone OIDC uses new dashboard flow
  * feat: activity requests are associated with child instance profiles
  * feat: grpc server accepts `SendCommandStatus` and publishes messages
  * feat: hostagent consumer processes command status messages
  * feat: set [api] cookie-encryption-key during standalone install/upgrade
  * feat: process account subdomains in middleware for API service
  * feat(appserver): redirect requests to invalid subdomains to the canonical url
  * feat: Add new API argument to return active and inactive interfaces
  * feat: traditional profiles are not applied to windows machines
  * fix: restrict GET /tags to caller's account
  * fix: handle extra emails with SSO
  * fix: remove serve-dashboard configuration
  * fix: allow parsing boolean config values
  * fix: parse boolean config values
  * fix: allow clearing tags of child instance profiles
  * fix: do not set JWT in local storage
  * fix: accept LANDSCAPE_SESSION_JWT cookie for auth
  * fix: allow standalone bootstrapping during OIDC flow
  * fix: include patch for improper PyCurl CA path in landscape-api client
  * fix: add request id to pending computer
  * fix: update link to script execution doc page
  * fix: route main button on /signup to /create-new-account

