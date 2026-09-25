# Multi-Tier Architecture - Two-Tier Architecture

A Two-Tier Architecture is a system that separates an application into two main parts: 
the Web/Application Tier and the Database Tier. These two tiers work together to process 
user requests and manage data.

## The Web/Application Tier
The web/application tier. It serves the user interface, handles HTTP 
requests, manages file uploads and downloads, and runs Nextcloud’s 
application logic. Users interact with this tier directly through port
8080.

## The Database Tier
The database tier stores persistent data such as user accounts, credentials,
file metadata, sharing permissions, and application state. It does not handle
web traffic directly and only responds to queries from the application tier.

## Why separate them?
Separating them lets each tier be updated or restarted independently
without affecting the other. It also improves security, since the
database doesn't need to be exposed to the internet. Finally, it keeps
the setup cleaner and easier to scale later.