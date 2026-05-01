<p align="center">
  <img src="https://raw.githubusercontent.com/ryujin-security/.github/refs/heads/main/picture/ryujin-logo.png" alt="Ryujin Security" width="160">
  <br>
  <strong>Ryujin Security</strong>
</p>

# Ryujin Security

Ryujin Security is an open-source security monitoring and web protection platform built around endpoint telemetry, centralized management, WAF protection, and security event visibility.

The project was created by **Reja Revaldy F** and **Ryan Rizky**.

## Repositories

| Repository | Description |
| --- | --- |
| [ryujin-agent](https://github.com/ryujin-security/ryujin-agent) | Endpoint agent for file integrity monitoring, system inventory, log collection, command monitoring, enrollment, and active response. |
| [ryujin-manager](https://github.com/ryujin-security/ryujin-manager) | Control plane for agent enrollment, certificate management, Coraza WAF, Quickwit event shipping, Sigma alerts, honeypot handling, and notifications. |
| [ryujin-dashboard](https://github.com/ryujin-security/ryujin-dashboard) | SvelteKit dashboard for agents, WAF sites, rules, honeypot credentials, security events, analytics, and notification settings. |

## Platform Overview

- Endpoint visibility through file integrity monitoring, command monitoring, inventory collection, and log collection.
- Secure agent enrollment with certificate-based identity.
- Web Application Firewall capabilities powered by Coraza and configurable rules.
- Security event pipelines for WAF logs, Sigma alerts, inventory, request logs, and active response data.
- Dashboard-driven operations for reviewing events and managing WAF configuration.
- Notification support for Telegram and Discord.

## Status

Ryujin Security is under active development. The current public release focuses on the core agent, manager, and dashboard components.

## Creators

- Reja Revaldy F
- Ryan Rizky
