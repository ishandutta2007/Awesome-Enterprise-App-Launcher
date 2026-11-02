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

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **Okta End-User Dashboard**

  **Application portal** within Okta identity platform. Users see assigned apps in a tile interface with SSO launch. **Pricing**: Quote-only; per-user and per-app models. **Free tier**: Developer edition available. **Best for**: Okta customers wanting a native app portal with conditional access—**trade-off**: requires Okta identity investment.



- **Microsoft My Apps**

  **Application launcher** within Entra ID (Azure AD). Users access assigned apps, manage groups, and request access. **Pricing**: Included with Entra ID; free tier limited. **Free tier**: Yes, with Entra ID Free. **Best for**: Microsoft-centric organizations wanting native SSO portal—**trade-off**: Microsoft ecosystem dependency.



- **OneLogin Portal**

  **Application portal** within OneLogin IAM. **Pricing**: Quote-only; tiered by users. **Free tier**: Trial available. **Best for**: OneLogin customers wanting a unified app launcher.



- **PingOne Dock**

  **Application launcher** within Ping Identity ecosystem. **Pricing**: Quote-only. **Free tier**: None. **Best for**: Ping customers wanting a personalized app dock.



- **JumpCloud User Portal**

  **Application portal** within JumpCloud directory. **Pricing**: Included with JumpCloud; tiered by users. **Free tier**: Yes, up to 10 users. **Best for**: JumpCloud users wanting SSO app access without Active Directory.



- **Rippling App Launcher**

  **Application access** within Rippling's unified HR/IT platform. **Pricing**: Quote-only; modular per-user pricing. **Free tier**: None. **Best for**: Rippling customers wanting apps alongside HR and device management.



- **Citrix Workspace**

  **Virtual app and desktop launcher** with SSO. **Pricing**: Quote-only; per-user. **Free tier**: None. **Best for**: enterprises needing virtualized app delivery alongside launcher—**trade-off**: infrastructure complexity; Citrix licensing costs.



- **VMware Workspace ONE**

  **Digital workspace platform** with app catalog and launcher. **Pricing**: Quote-only; per-user. **Free tier**: None. **Best for**: VMware-centric enterprises wanting unified endpoint and app management—**trade-off**: Broadcom acquisition uncertainty.



- **Workgrid**

  **Digital workplace assistant** with app launcher and communications. **Pricing**: Quote-only. **Free tier**: None. **Best for**: enterprises wanting a modern intranet-style app hub.



- **Atlassian Start**

  **Note**: No public information found for an Atlassian "Start" app launcher product in available search results. Atlassian offers Home (workspace hub) but not a standalone enterprise app launcher. **Best for**: verify directly with Atlassian before evaluating.



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
