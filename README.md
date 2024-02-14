# Microsoft Sentinel Learning Collection

Microsoft Sentinel is cloud native SIEM/SOAR solution. It is a SaaS based solution, published on top of Log Analytics workspace
- SIEM — Security Information and Event Management
- SOAR — Security Orchestration, Automation and Response.

This repository is the collection of links which can help you get started with Sentinel

## Planning and Onboarding
### Video sessions 
I recommend these 2 videos if you are new to Sentinel. These explain the architecture as well as features details
- https://www.youtube.com/watch?v=xu7UIRJ7tBw&pp=ygUabWljcm9zb2Z0IHJlYWN0b3Igc2VudGluZWw%3D
- https://www.youtube.com/watch?v=xMj7a4Ns_cU&pp=ygUabWljcm9zb2Z0IHJlYWN0b3Igc2VudGluZWw%3D

### Design Considerations
Before starting setting up Sentinel, it is important to understand the cost, logs, access and best practices. Use these links to understand the best solution for your needs
- [Design your Microsoft Sentinel workspace architecture | Microsoft Learn](https://learn.microsoft.com/en-us/azure/sentinel/design-your-workspace-architecture)
- [Roles and permissions in Microsoft Sentinel | Microsoft Learn](https://learn.microsoft.com/en-us/azure/sentinel/roles)
- [Sample Microsoft Sentinel workspace designs | Microsoft Learn](https://learn.microsoft.com/en-us/azure/sentinel/sample-workspace-designs)
- [Quickstart: Onboard in Microsoft Sentinel | Microsoft Learn](https://learn.microsoft.com/en-us/azure/sentinel/quickstart-onboard)

### Cost Considerations
- [Manage and monitor costs for Microsoft Sentinel | Microsoft Learn](https://learn.microsoft.com/en-us/azure/sentinel/billing-monitor-costs)
- [Enroll in a simplified pricing tier for Microsoft Sentinel | Microsoft Learn](https://learn.microsoft.com/en-us/azure/sentinel/enroll-simplified-pricing-tier?tabs=microsoft-sentinel)
- [Reduce costs for Microsoft Sentinel | Microsoft Learn](https://learn.microsoft.com/en-us/azure/sentinel/billing-reduce-costs)

### Best Practices
[Best practices for Microsoft Sentinel | Microsoft Learn](https://learn.microsoft.com/en-us/azure/sentinel/best-practices)https://learn.microsoft.com/en-us/azure/sentinel/best-practices

## Data Connectors/Analytics/Incident Management
Data connectors are the data sources which ingest your data to Microsoft Sentinel. Once ingested you can use the analytics to set up incidents and alerts on the ingested data.
Note:Sentinel works on top of log analytics workspace. Thus familiarity with KQL (Kusto Query Language) is required to query the tables. These links will help you get started with Data connectors and analytics
- [Microsoft Sentinel data connectors | Microsoft Learn](https://learn.microsoft.com/en-us/azure/sentinel/connect-data-sources)
- [Detect threats with analytics rule templates in Microsoft Sentinel | Microsoft Learn](https://learn.microsoft.com/en-us/azure/sentinel/detect-threats-built-in)
- [Custom data ingestion and transformation in Microsoft Sentinel | Microsoft Learn](https://learn.microsoft.com/en-us/azure/sentinel/data-transformation)
- [Microsoft Sentinel content hub catalog | Microsoft Learn](https://learn.microsoft.com/EN-US/azure/sentinel/sentinel-solutions-catalog)
- [What is a watchlist - Microsoft Sentinel | Microsoft Learn](https://learn.microsoft.com/en-us/azure/sentinel/watchlists)
- [Best practices for data collection in Microsoft Sentinel | Microsoft Learn](https://learn.microsoft.com/en-us/azure/sentinel/best-practices-data)
- [Find your Microsoft Sentinel data connector | Microsoft Learn](https://learn.microsoft.com/en-us/azure/sentinel/data-connectors-reference)

## Threat Hunting and Intelligence
- [Advanced multistage attack detection in Microsoft Sentinel | Microsoft Learn](https://learn.microsoft.com/en-us/azure/sentinel/fusion)
- [Threat intelligence integration in Microsoft Sentinel | Microsoft Learn](https://learn.microsoft.com/en-us/azure/sentinel/threat-intelligence-integration)
- [Use matching analytics to detect threats - Microsoft Sentinel | Microsoft Learn](https://learn.microsoft.com/en-us/azure/sentinel/use-matching-analytics-to-detect-threats)

## Archival and Restoring of Logs
Cost becomes an important factor with the increase of log ingestion, these links can help you with data archival and restore in different resources
- Log Analytics Workspace - 
[Data retention and archive in Azure Monitor Logs - Azure Monitor | Microsoft Learn](https://learn.microsoft.com/en-us/azure/azure-monitor/logs/data-retention-archive?tabs=portal-1%2Cportal-2)
[Run search jobs in Azure Monitor - Azure Monitor | Microsoft Learn](https://learn.microsoft.com/en-us/azure/azure-monitor/logs/search-jobs?tabs=portal-1%2Cportal-2)
[Restore logs in Azure Monitor - Azure Monitor | Microsoft Learn](https://learn.microsoft.com/en-us/azure/azure-monitor/logs/restore?tabs=api-1)
- Storage Accounts 
[Access tiers for blob data - Azure Storage | Microsoft Learn](https://learn.microsoft.com/en-us/azure/storage/blobs/access-tiers-overview)
- Comparison of other options
https://techcommunity.microsoft.com/t5/microsoft-sentinel-blog/a-look-at-different-options-for-storing-and-searching-sentinel/ba-p/3713698


## Workbooks 
- Workbooks help you to visualize and monitor data once your data source is connected to the Sentinel. You can use pre-defined templates or create your own workbooks. Some workbook templates also comes with "guide"  option to help you set up the workbooks.
- Here are some of the predefined workbooks templates in the content hub which help you streamline your experience with Sentinel.
    -  [Soc Process Framework](https://techcommunity.microsoft.com/t5/microsoft-sentinel-blog/what-s-new-soc-process-framework-is-now-live-in-content-hub/ba-p/3590349). With deployment of this solution you can monitor progress with you SOC operatios and update the SOC CMMI assessment score.
    -  [Zero trust TIC 3.0](https://techcommunity.microsoft.com/t5/public-sector-blog/announcing-the-azure-sentinel-zero-trust-tic3-0-workbook/ba-p/2313761) This solution provides a visulization of Zero Trust principles cross walked to the Trusted Internet Connections framework.
    -  Microsoft Sentinel cost -  This workbook provides an estimated cost across the main billed items in Microsoft Sentinel: ingestion, retention and automation. It also provides insight about the possible impact of the Microsoft 365 E5 offer.
    -  [Security Operations efficiency workbook](https://learn.microsoft.com/en-us/azure/sentinel/manage-soc-with-incident-metrics). This is the outof box workbook aimned to improve security operations efficiency by providing metrics such as: incident created over time, mean time to triage, mean time to closure etc.
    -  [Other commonly used Microsoft Sentinel Wworkbooks](https://learn.microsoft.com/en-us/azure/sentinel/top-workbooks)
### Workbooks with Power BI
 [Create a Power BI report from Microsoft Sentinel data | Microsoft Learn](https://learn.microsoft.com/en-us/azure/sentinel/powerbi)

## Sentinel Blogs
A useful link to understand different use case
https://techcommunity.microsoft.com/t5/microsoft-sentinel-blog/bg-p/MicrosoftSentinelBlog

## Sentinel Training Lab (Available in Sentinel Content Hub)
For hands on lab, this is a fantastic content hub solution you can utilize [Microsoft Sentinel Training Lab](https://github.com/Azure/Azure-Sentinel/tree/master/Solutions/Training/Azure-Sentinel-Training-Lab).

## A new article, summarizing all the Sentinel 100 information:
https://techcommunity.microsoft.com/t5/fasttrack-for-azure/microsoft-sentinel-soar-through-the-siem-begin-with-the-basics/ba-p/3990142

## Other GitHub Repos
- Sentinel All in One
[Azure-Sentinel/Tools/Sentinel-All-In-One at master · Azure/Azure-Sentinel (github.com)](https://github.com/Azure/Azure-Sentinel/tree/master/Tools/Sentinel-All-In-One)
- KQL Queries
[reprise99/Sentinel-Queries: Collection of KQL queries (github.com)](https://github.com/reprise99/Sentinel-Queries)
- Sentinel as code
[sreedharande/Microsoft-Sentinel-As-A-Code: Export Microsoft Sentinel artifacts like Analytical Rules, Hunting Queries, Workbooks in order to support new feature Repositories CI/CD Pipeline (github.com)](https://github.com/sreedharande/Microsoft-Sentinel-As-A-Code/tree/main)
- Sentinel for SOC
[briandelmsft/SentinelAutomationModules: The Microsoft Sentinel Triage AssistanT (STAT) enables easy to create incident triage automation in Microsoft Sentinel (github.com)](https://github.com/briandelmsft/SentinelAutomationModules) <br>
[rod-trent/Sentinel-SOC-101: Content and collateral for the Microsoft Sentinel SOC 101 series (github.com](https://github.com/rod-trent/Sentinel-SOC-101)
- **Threat Hunting**: 
<ol>
<li>https://github.com/cyb3rmik3/KQL-threat-hunting-queries/tree/main </li>
<li>https://github.com/Bert-JanP/Hunting-Queries-Detection-Rules/tree/main
<li>https://github.com/Azure/Azure-Sentinel-Notebooks
<li>https://learn.microsoft.com/en-us/azure/sentinel/notebooks-hunt?tabs=public-endpoint</li> </ol>


