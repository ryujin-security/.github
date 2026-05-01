# Ryujin Security

Ryujin Security is an open-source security monitoring and web protection platform built around endpoint telemetry, centralized management, WAF protection, and security event visibility.

The project was created by **Reja Revaldy F** and **Ryan Rizky**.

## System Architecture
<p align="center">
<img  width="884" height="515" alt="image" src="https://github.com/user-attachments/assets/9e0e6820-1baa-4692-928e-ed53b0905770" />
</p>
## Repositories

| Repository                                                              | Description                                                                                                                                          |
| ----------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
| [ryujin-agent](https://github.com/ryujin-security/ryujin-agent)         | Endpoint agent for file integrity monitoring, system inventory, log collection, command monitoring, enrollment, and active response.                 |
| [ryujin-manager](https://github.com/ryujin-security/ryujin-manager)     | Control plane for agent enrollment, certificate management, Coraza WAF, Quickwit event shipping, Sigma alerts, honeypot handling, and notifications. |
| [ryujin-dashboard](https://github.com/ryujin-security/ryujin-dashboard) | SvelteKit dashboard for agents, WAF sites, rules, honeypot credentials, security events, analytics, and notification settings.                       |

## Platform Overview

* Endpoint visibility through file integrity monitoring, command monitoring, inventory collection, and log collection.
* Secure agent enrollment with certificate-based identity.
* Web Application Firewall capabilities powered by Coraza and configurable rules.
* Security event pipelines for WAF logs, Sigma alerts, inventory, request logs, and active response data.
* Dashboard-driven operations for reviewing events and managing WAF configuration.
* Notification support for Telegram and Discord.

## Background

Ryujin Security is developed as a final project at a polytechnic institution and published as an open-source platform. The system is still evolving, with known limitations and areas requiring further improvement in architecture, performance, and feature completeness.

## Status

Ryujin Security is under active development. The current public release focuses on the core agent, manager, and dashboard components.

## Creators

* Reja Revaldy F

  * LinkedIn: [https://www.linkedin.com/in/rejarevaldyf/](https://www.linkedin.com/in/rejarevaldyf/)
  * GitHub: [https://github.com/rejarevaldy](https://github.com/rejarevaldy)

* Ryan Rizky

  * LinkedIn: [https://www.linkedin.com/in/ryanriz/](https://www.linkedin.com/in/ryanriz/)
  * GitHub: [https://github.com/ryanriz](https://github.com/ryanriz)
