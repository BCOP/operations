# Issue Tracking Systems

## Overview

Issue tracking systems are often present as part of both internal and external workflows at IT departments of a wide range of organizations, and are commonly used for various aspects of network operations in the context of autonomous systems.

While some organizations use issue tracking systems sparingly, primarily in customer support functions such as help desk issue tracking, others use them as a general "message queue for humans", sometimes with elaborate workflow rules, in place of a workflow engine.

The following processes in autonomous systems operations are often managed via issue tracking systems:

* Tracking of inbound and outbound communication with customers (support@)
* Tracking of inbound and outbound communication with peers (peering@)
* Tracking of inbound abuse reports (abuse@)

Some particularly lean service providers targeting technically sophisticated customers are using an issue tracking system to manage inbound sales requests (sales@) and the entire sales process, and use the user registration of the issue tracking system instead of a CRM.

Other ASes, especially those dealing primarily with internal users (such as a networking department of a larger non-internet service provider, on-line media agencies, etc.) or those with a limited number of customer relationships but deep and broad engagements (such as boutique service providers targeting enterprises with unique needs in specific verticals) find a project management system with a limited e-mail interface to be a good replacement for a ticketing system.

Such systems often have better dependency management and workflow capabilities built in, which lend themselves better to management of more complex, long-lasting issues.

## Recommendations

### Pure-Play Ticketing Systems
* [Freshdesk](https://www.freshdesk.com) - Simple ticketing system suitable for a wide range of processes with emphasis on ease of use and self-service. Handles e-mail parsing well. SaaS.
* [ZenDesk](https://www.zendesk.com/) - Extensive ticketing system with strong [Salesforce](https://www.salesforce.com/) integration. SaaS.
* [Zoho Support](https://www.zoho.com/support/) - Extensive ticketing system that works well with Zoho's other tools and can form part of a more comprehensive process automation and project management toolset. SaaS or self-hosted.

### Project Management Tools with Ticketing Capability
* [JIRA](https://www.atlassian.com/software/jira) - Atlassian JIRA is an issue tracking and project management system that forms a part of a larger suite of tools from Atlassian. SaaS or self-hosted.
* [Taskray](https://www.taskray.com/) - A flexible project management system that's sufficiently agile for smaller issues. SaaS.
* [Basecamp](https://www.basecam.com/) - Basecamp 3 is a project management system that can be easily exposed to customers for managing singular issues or multi-element projects with dependencies and workflows. SaaS.

## Do and Don't

### Do:
* Craft professionally written canned responses for common situations. Translate these canned responses into the most common languages used in your ASes service region. This allows agents to communicate consistently and communicate in a foreign language with which they may have limited familiarity without risking unnecessary misunderstandings.

* Expore utilizing a dedicated abuse management system for abuse@, as such systems often have specialty functions that greatly simplify abuse response which would be difficult to replicate in an issue tracking or project management system.

### Don't:
* Don't enable any form of confirmation or auto-responders on ticketing systems tied to e-mail addresses used for mailing lists. It's not uncommon for a growing organizations to register a noc@ or similar e-mail role distribution list for mailing lists so that the information is disseminated to all relevant personnel in the organization, and subsequently re-route the alias to a ticketing system. This can cause acknowledgement e-mails from the ticketing system to be sent to the mailing list and greatly inconvenience a surprisingly large number of people in a very short time.

* Don't expose a ticketing system as the sole entry point of contact for your organization or functional group; ticketing systems get overloaded, break, parse some forms of content poorly, and might mis-classify or mis-prioritize inbound requests. Always offer a secondary channel into your organization (phone, fax, IRC channel, ...)
