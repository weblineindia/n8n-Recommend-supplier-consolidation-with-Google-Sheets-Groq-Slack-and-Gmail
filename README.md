# AI Supplier Consolidation Analysis with Google Sheets, Groq, Slack & Gmail

## Quick Overview

This workflow runs weekly to analyze supplier spend data from Google Sheets, identify overlapping suppliers across departments, estimate potential consolidation savings, and use Groq AI to evaluate procurement risks and generate recommendations. The workflow then sends actionable insights to Slack and emails personalized reports to supplier stakeholders.

---

## How it works

1. Runs automatically every week using a scheduled trigger.
2. Reads supplier procurement data from Google Sheets, including supplier name, department, monthly spend, risk rating, and stakeholder email.
3. Normalizes supplier names, detects suppliers shared across multiple departments, and calculates estimated consolidation savings and opportunity levels.
4. Sends each consolidation opportunity to a Groq AI model, which evaluates procurement risk, savings potential, and recommends the best consolidation strategy.
5. Parses the structured AI response and combines it with the calculated procurement metrics.
6. Posts a formatted recommendation to Slack for procurement visibility.
7. Emails a personalized consolidation report and AI recommendations to the relevant supplier stakeholder.

---

## Setup

1. Connect Google Sheets OAuth2 credentials and configure the spreadsheet ID and worksheet containing supplier procurement data.
2. Add Groq API credentials and select the preferred language model for procurement analysis.
3. Connect Slack OAuth2 credentials and select the channel for consolidation alerts.
4. Connect Gmail OAuth2 credentials and configure recipient emails using the stakeholder email column or specify a fixed recipient.
5. Review the savings calculation logic and supplier normalization rules to match your procurement policies.

---

## Requirements

- **[n8n account (Self-hosted or Cloud)](https://n8n.partnerlinks.io/om1efg2qgvwi)**
- Google Sheets account
- Groq API credentials
- Slack workspace with OAuth2 credentials
- Gmail account with OAuth2 credentials
- Supplier spend data including supplier name, department, monthly spend, risk rating, and stakeholder email

---

## Customization

### Schedule Trigger

Customize:

- Weekly schedule
- Daily or monthly execution
- Custom Cron expressions

### Data Source

Replace Google Sheets with:

- Airtable
- MySQL
- PostgreSQL
- Microsoft SQL Server
- SAP exports
- Oracle ERP
- CSV imports

### Savings Calculation

Customize:

- Minimum spend thresholds
- Savings percentage calculations
- Opportunity scoring
- Department grouping rules
- Supplier normalization logic

### AI Prompt

Extend the analysis by including:

- ESG scores
- Supplier performance history
- Compliance ratings
- Contract renewal dates
- Delivery performance
- Financial health
- Geographic risk
- Supplier diversity metrics

### Notifications

Replace or extend notifications with:

- Microsoft Teams
- Discord
- WhatsApp
- SMS
- Jira
- ServiceNow
- CRM updates
- Procurement platforms

---

## Additional Info

### Who's It For

- Procurement teams
- Strategic sourcing managers
- Finance departments
- Supply chain managers
- Vendor management teams
- Operations leaders
- Enterprise procurement organizations

---

## Add-Ons & Enhancements

- Automated procurement ticket creation
- Vendor negotiation reports
- Power BI dashboards
- Looker Studio reporting
- SAP integration
- Oracle ERP synchronization
- Multi-country supplier scoring
- Contract renewal monitoring
- Approval workflows
- Historical procurement analytics
- Executive PDF reports
- Cost-saving trend analysis

---

## Use Case Examples

1. Identify duplicate software vendors across IT departments.
2. Consolidate office supply vendors to negotiate better pricing.
3. Optimize logistics providers across multiple business locations.
4. Rationalize marketing agencies used across departments.
5. Consolidate manufacturing suppliers to leverage bulk purchasing discounts.
6. Improve procurement compliance across business units.
7. Support strategic sourcing initiatives using AI-powered recommendations.

There are many additional use cases depending on your procurement processes, supplier network, and sourcing strategy.

---

## Troubleshooting Guide

| Issue | Possible Cause | Solution |
|--------|----------------|----------|
| Workflow does not run | Workflow is inactive | Activate the workflow and verify the schedule |
| Google Sheets connection fails | OAuth credentials expired | Reconnect Google Sheets credentials |
| No suppliers detected | Incorrect spreadsheet structure | Verify worksheet and column mappings |
| Supplier overlaps not identified | Supplier names are inconsistent | Improve supplier name normalization logic |
| AI response parsing fails | Invalid or unexpected AI output | Update the AI prompt to enforce structured JSON |
| Slack notification fails | Incorrect Slack configuration | Reconnect Slack credentials and verify channel permissions |
| Email notifications fail | Gmail OAuth expired | Reconnect Gmail credentials |
| Savings estimates appear incorrect | Invalid spend data | Validate monthly spend values and calculation logic |

---

## Need Help?

If you need help customizing this workflow, integrating it with your procurement ecosystem, or extending it with AI-powered supplier analytics, ERP integrations, approval workflows, negotiation support, and executive reporting, our **WeblineIndia** team is ready to assist.

Explore our **[Process Automation Solutions](https://www.weblineindia.com/process-automation-solutions.html)** or connect with our **[n8n workflow development experts](https://www.weblineindia.com/n8n-automation/)** to build, customize, and scale your business automation with confidence.
