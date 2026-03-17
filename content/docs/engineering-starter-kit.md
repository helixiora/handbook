+++
title = "Engineering Starter Kit"
date = 2026-03-16T21:05:00+01:00
weight = 12
kicker = "Engineering"
lead = "Engineers should be able to get from a fresh company laptop to a secure, usable baseline without chasing setup advice in chat."
description = "Default engineering laptop, account, and tool baseline for Helixiora."
owner = "technology"
applies_to = "Engineers and technical contributors"
+++

## What this page is for

This page defines the default Helixiora engineering starter kit. Use it to set up a company laptop, confirm account access, and avoid repeating the same onboarding instructions in private chat.

Because Helixiora works in consulting, client context may add extra tools. Start with this baseline first, then add only the project-specific tools the customer actually requires.

## Day-one non-negotiables

Before you start normal engineering work, make sure all of the following are true:

1. You can sign in to 1Password, Slack, Google Workspace, ClickUp, and GitHub.
2. MFA or 2FA is enabled on every work account that supports it.
3. Work passwords and secrets live in 1Password rather than in the browser.
4. Your laptop has full-disk encryption, automatic locking, and OS updates enabled.
5. You know who to contact for access problems: Technology lead (Walter) first, then People lead (Robin) if Walter is unavailable.

## Default toolkit

| Category | Standard | When it applies |
| --- | --- | --- |
| Identity and secrets | 1Password, MFA or 2FA, separate work browser profile | Always |
| Communication and planning | Slack, Google Workspace, ClickUp | Always |
| Code and collaboration | GitHub, local Git setup, pull-request workflow | Always |
| Local development | One primary editor or IDE, one primary terminal, and a container runtime when the project needs local services or reproducible builds | Most engineering roles |
| Language runtimes and package managers | Install only the runtimes and package managers required by the current project | Per project |
| Cloud and infrastructure access | AWS, Azure, Hetzner, Linode, VPNs, and CLI tools only for the environments you actually touch | Per project |
| AI tooling | Use the tools approved under [AI & Experimentation](/docs/ai-and-experimentation/) and respect client restrictions | When allowed |
| Time and admin | Harvest, Deel, and contract-specific admin routes where relevant | Only if your work or contract requires it |

## Laptop baseline

Use this as the default machine setup:

- Keep a separate work browser profile so company and client accounts stay isolated from personal browsing.
- Install one terminal you will use consistently and one primary editor or IDE you can support yourself in.
- Keep Git available locally and confirm you can clone, commit, and open pull requests in the Helixiora GitHub organization.
- Install a container runtime only when your current project needs it.
- Add only the language toolchains your active project uses instead of preloading every ecosystem.
- Keep local notes, scratch files, and exported client data inside approved work locations rather than on random desktop folders.

## Project-specific add-ons

Depending on the customer or project, you may also need:

- VPN or zero-trust access tooling
- Cloud CLIs or SSO tooling
- Database clients
- Local service emulators
- Mobile tooling or simulators
- Design or analytics tools that support the delivery team

If a project needs one of these, add it deliberately and document it in the project README, onboarding task, or internal setup notes so the next engineer does not have to rediscover it.

## Working rules

- Start from the Helixiora baseline, then adapt to the client instead of the other way around.
- Keep company and client accounts separated wherever the tooling allows it.
- Avoid installing powerful infrastructure tools "just in case"; request access when there is a real delivery need.
- If you are missing a baseline tool or approval, raise it early instead of blocking silently.

## What good looks like after week one

By the end of your first week, you should be able to:

1. Access every repo, workspace, and communication channel needed for your current assignment.
2. Run the main project locally or use the agreed remote development environment.
3. Open a pull request, comment on work, and follow the team review path.
4. Explain which tools are Helixiora defaults and which ones are customer-specific exceptions.
