# Awesome-Enterprise-App-Launcher

# Awesome-Enterprise-App-Launcher

**Top Enterprise App Launcher (Opensource) 🌟 Star if you like it! 🌟**



**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on SSO Portals, Application Dashboards, Virtual Desktop Launching & Self-Hosted Access Hubs*

**Last updated: November 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Enterprise App Launcher**. These tools provide employees with a single portal to access their applications—handling SSO, app discovery, and launch without requiring users to remember dozens of URLs—from fully managed identity dashboards with conditional access to open-source launchers that give organizations control over their access hub.



**Examples** include Okta End-User Dashboard, Microsoft My Apps, OneLogin Portal, PingOne Dock, JumpCloud User Portal, Rippling, Citrix Workspace, VMware Workspace ONE, Workgrid, and Atlassian Start (the category leaders in commercial space).



**Open-source emphasis**: This section is expanded with every relevant project for self-hosted app launchers, SSO portals, and open access infrastructure. **Critical note**: True open-source enterprise app launchers are rare—**Heimdall** is the most mature application dashboard for self-hosted services , **appswitcher-server** provides a Keycloak-integrated launcher bar , and **Pocket ID Dashboard** adds a community-built portal layer to a lightweight IdP . No open-source project matches Okta's conditional access or Citrix's virtual app streaming, but for simple SSO app portals, the options are functional.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## Sector Overview & Market Dynamics

The enterprise app launcher, SSO portal, and digital identity workspace market is valued between $25 billion and $30 billion globally, projected to exceed $70 billion over the next decade at a ~12–15% CAGR driven by zero-trust security initiatives and hybrid workplace sprawl. The sector exhibits a bifurcated structure: while moderately fragmented across niche self-hosted portals and point SSO utilities, enterprise adoption is heavily concentrated among massive hyperscalers and identity platforms (notably Microsoft and Okta) that drive winner-take-most dynamics through deep workplace ecosystem lock-in.

## SaaS/Hosted Platforms

| Product | Company Valuation / Revenue | Pricing (Starting Tier) | Free Tier / Trial Limits | Description & Best For |
| :--- | :--- | :--- | :--- | :--- |
| **Microsoft My Apps** | ~$3.88 Trillion (Market Cap) | $0 (included with Entra ID Free); Paid tiers start at $7.00/user/mo (Entra ID P1) | Free forever up to 50,000 directory objects (expands to 300,000 objects with custom domain; no conditional access SLA); Paid tiers offer 30-day free trial | Application launcher within Microsoft Entra ID. Best for Microsoft-centric organizations needing native SSO app launching. |
| **Atlassian Start / Home** | ~$52 Billion (Market Cap) / ~$6.57B ARR | Free with Atlassian Cloud; core plans start at $7.75/user/mo (Jira Standard) | Free forever up to 10 users per Atlassian product instance; Paid tiers offer 7-to-30-day free trial | Centralized workspace navigation and cross-product launcher across Jira, Confluence, and Atlassian Cloud. |
| **Okta End-User Dashboard** | ~$38 Billion (Market Cap) / ~$3.0B ARR | $6.00/user/mo (Workforce Identity Starter tier, annual billing, ~$1,500 annual minimum) | 30-day free trial with full platform access (SSO, MFA, Universal Directory); Developer edition free tier available | Dedicated enterprise tile launcher within Okta Workforce Identity Cloud with granular access controls. |
| **Rippling App Launcher** | $16.8 Billion (Valuation) / >$1.0B ARR | $8.00/user/mo (Core Unity platform) + ~$6.00/user/mo (IAM & App Access module) | No free forever tier; provides interactive product tours and pilot trial access on request (no self-serve free trial) | Unified identity and application access portal integrated directly into HR, payroll, and IT endpoint workflows. |
| **Citrix Workspace** | $16.5 Billion (Acquisition Valuation) / ~$3.2B Revenue | $10.00/user/mo (Citrix DaaS Standard starting tier, BYO cloud infrastructure) | No free forever tier; Proof-of-concept enterprise trial available upon request via sales partners (typically 30-day trial) | Virtual application and desktop launcher combining SSO tile access with remote application delivery. |
| **PingOne Dock** | $16.5 Billion (Acquisition Valuation by Thoma Bravo) / ~$300M Revenue | $3.00/user/mo (PingOne for Workforce Essential tier; typically 5,000 user minimum contract) | 30-day free trial with authentication, MFA, and SSO directory access; no permanent free tier | Employee dock and application launchpad within Ping Identity's workforce IAM ecosystem. |
| **Omnissa / VMware Workspace ONE** | $4.0 Billion (Acquisition Valuation by KKR) / ~$1.5B ARR | $3.00/user/mo (Employee Essentials tier for identity, SSO, and app catalog) | No free forever tier; 30-day proof-of-concept evaluation trial available via Omnissa sales channels | Digital workspace app catalog combining unified endpoint management with an enterprise application launcher. |
| **JumpCloud User Portal** | $2.63 Billion (Valuation) | $9.00/user/mo (Device Management) or $11.00/user/mo (SSO package) | 30-day full-feature free trial (legacy accounts created before Feb 2024 have 10 users / 10 devices free limit) | Cloud directory user portal delivering SSO application access without requiring Active Directory. |
| **OneLogin Portal** | ~$500 Million (Acquisition Valuation by One Identity) / ~$25M Revenue | $2.00/user/mo (Starter Directory/Workflows entry tier); Advanced SSO bundles from ~$4–$8/user/mo | 30-day free trial with complete SSO and portal capabilities; no permanent free production tier | Single-sign-on application launchpad and cloud directory within OneLogin IAM. |
| **Workgrid** | Wholly-owned subsidiary of Liberty Mutual ($50B+ Revenue); ~$5M standalone ARR scale (wound down mid-2025) | ~$5.00/user/mo (Baseline enterprise digital assistant entry tier, custom enterprise quote) | Custom pilot evaluation trial available on request (no self-serve free forever tier) | Digital workplace assistant with an embedded micro-app launcher and notification stream. |



## Open-Source GitHub Projects



- **Heimdall**

  **Application dashboard and launcher** (MIT, linuxserver.io) — **the most mature open-source app dashboard** for self-hosted services and web applications . **Features**: **Organize all your web apps and services in one place**; icon-based tile interface; search and categorization; Docker deployment (Podman CLI, Compose examples provided) . **Tech stack**: PHP (Laravel). **Deploy**: Self-hosted (Docker, Podman) or linuxserver.io container. **Trade-off**: **Dashboard for self-hosted services, not an SSO portal**—it links to apps but does not handle authentication or conditional access. **Best for**: homelabs and small teams wanting a visual launchpad for their self-hosted apps—especially those already using linuxserver.io containers.



- **appswitcher-server**

  **Icon-based application switcher for embedding in corporate web apps** (open source, it@M Munich) — **the most enterprise-oriented open-source launcher**, designed to be embedded via iframe into existing applications . **Features**: **Configure applications** via YAML with name, URL, icon, and sort order; **tags** for domain filtering (`finance`, `development`, etc.); **Keycloak integration**—apps only appear if the user's access token audience includes the configured client ID; **embed via iframe** with tag-based filtering (e.g., `?tags=development`) . **Tech stack**: Spring Boot (Java), Vue.js/Vuetify components available. **Deploy**: Self-hosted (Spring Boot application). **Trade-off**: **Launcher bar, not a full portal**—it provides the app-switching UI, not a standalone dashboard or SSO engine. **Best for**: organizations using Keycloak wanting a Google App Bar-style switcher embedded in their internal web applications—especially those wanting permission-aware app visibility.



- **Pocket ID Dashboard**

  **Community-built dashboard for Pocket ID OIDC clients** (open source, community project) — **the most focused open-source Okta Dashboard alternative** for lightweight IdPs . **Features**: **Dashboard for users to view all their OIDC clients**; **access request workflow**—users can request access to clients they don't yet have; **admin features** via user group designation; **PKCE flow** for security; **Docker image** available . **Tech stack**: Node.js, VueJS (NuxtUI). **Deploy**: Self-hosted (Docker, ghcr.io). **Trade-off**: **Community project**—not an official Pocket ID feature; requires Pocket ID as the IdP. **Best for**: Pocket ID users wanting a dashboard and access request experience—especially homelabs and small teams using Pocket ID for SSO.



- **Beeline**

  **Fast, keyboard-first launcher for Microsoft My Apps / Entra SSO apps** (MIT, browser extension) — **the most focused launcher for Microsoft-centric users**, built as a lightweight alternative to the official My Apps Secure Sign-in extension . **Features**: **Instant**—renders from local storage, no network round-trip; **keyboard-first**—fuzzy search, arrow keys, Enter to launch; **learns habits**—most-used and recent apps rise to top; **sync with My Apps**—pulls tiles from `myapplications.microsoft.com`; **private by design**—no telemetry, no analytics; **Fallback search**—search My Apps or web when no match . **Tech stack**: JavaScript (browser extension). **Deploy**: Browser extension (Firefox, Chrome). **Trade-off**: **Launcher only**—does not replace Entra's password vaulting or credential auto-fill; apps open via normal SSO flow. **Best for**: Microsoft 365 users wanting faster access to their SSO apps without navigating the My Apps portal—especially those who launch the same few apps daily.



### Additional Strong Open-Source Options



- **openSME Portal** — Custom Rust/Axum landing page within openSME digital workplace stack (open source). Service directory for a self-hosted suite including Zitadel SSO, OpenCloud, Collabora, and others . **Note**: **Portal for a specific stack**—not a general app launcher; requires openSME deployment. **Best for**: teams deploying the full openSME stack wanting a pre-built landing page.

- **Kanidm Application Portal** — Application portal within Kanidm identity management (MPL-2.0). Allows easy access to linked applications alongside OAuth2/OIDC SSO . **Note**: **Portal component of an IdP**—requires Kanidm deployment. **Best for**: Kanidm users wanting an integrated app portal with their identity provider.

- **Mijn Bureau** — Dutch government open-source digital workplace suite (open source). Includes Keycloak, Nextcloud, Element, and other components with a unified portal . **Note**: **Full workplace suite**, not a standalone launcher. **Best for**: public sector organizations wanting a sovereign workplace with app access.



**Frameworks for building custom systems**: Combine **Heimdall** for a visual dashboard with **appswitcher-server** for Keycloak-integrated embedding and **Beeline** for Microsoft-centric quick launch—creating a layered app launcher stack. **None of these match Okta's conditional access or Citrix's virtual app delivery**, but for SSO portal and quick launch needs, the options are functional.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, license (for open-source), and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- App launcher platforms handling SSO and access permissions must comply with data protection regulations (GDPR, CCPA, etc.) and implement appropriate access controls.

- **The "identity-native portal" vs. "self-hosted dashboard" vs. "embedded launcher" vs. "browser extension" distinction is critical.** **Okta, Microsoft My Apps, OneLogin, PingOne, JumpCloud, Rippling, Citrix, VMware, and Workgrid** are **identity-native portals**—they are part of an IAM or workspace platform and leverage its SSO and access controls . **Heimdall** is a **self-hosted dashboard**—it provides a visual launchpad but does not handle authentication . **appswitcher-server** is an **embedded launcher**—it is designed to be iframed into existing apps with Keycloak permission awareness . **Beeline** is a **browser extension**—it accelerates access to Microsoft My Apps but does not replace the portal . **Choose based on whether you need managed SSO, a visual launchpad, embedded switching, or quick access.**

- **Heimdall is the most mature open-source app dashboard** for self-hosted services—it organizes links to your apps in a clean tile interface . **The trade-off**: it is not an SSO portal; it does not authenticate or authorize users. **For homelabs and internal tools, it is the pragmatic choice.**

- **appswitcher-server is the most enterprise-oriented open-source launcher**—it integrates with Keycloak to show only apps a user can access, and embeds via iframe like Google's App Bar . **The trade-off**: it is a launcher bar, not a full portal; requires Keycloak.

- **Pocket ID Dashboard is a community project**, not an official Pocket ID feature. **The trade-off**: requires Pocket ID as the IdP; community-maintained. **For Pocket ID users, it fills a real gap**—Pocket ID itself is a lightweight IdP without a user dashboard.

- **Beeline is the most practical launcher for Microsoft 365 users**—keyboard-first, instant, and private, with no telemetry . **The trade-off**: it is a browser extension, not a portal replacement; apps open via normal SSO.

- **Atlassian Start could not be verified** as a standalone app launcher product in available search results. **Verify directly with Atlassian before including it in any evaluation.**

- Self-hosted open-source solutions require proper infrastructure (PHP for Heimdall, Java for appswitcher-server, Node.js for Pocket ID Dashboard), security hardening, and ongoing maintenance. **App launchers expose links to internal systems**—ensure your deployment meets your organization's security requirements before exposing application URLs.



---



**Made for IT administrators, identity engineers, and organizations building transparent app launcher solutions.**

Let's make Enterprise App Launchers more open, data-driven, and SSO-aware.
