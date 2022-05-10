# 0005. Observability tools and strategy

Date: 2021-06-18

## Status

Accepted

## Context

We need to be able to monitor our solution, and be notified by automated alerts when problems occur.

## Decision

We will base our solution around Azure Monitor and its related services. As a managed service, it means:

- Scaling, updates and data storage are taken care of as part of the solution, resulting in lower running costs.
- It is an Azure native service and thus simple to configure as it already integrates with the key services we intend to use

### Metrics

We will use [Azure Monitor Metrics](https://docs.microsoft.com/en-us/azure/azure-monitor/essentials/data-platform-metrics) to collect metrics for our solution.  

- The service 'collects' and stores numerical metric data in a time-series database for ease of query
- Azure Monitor Metrics can be easily used for Alerting, Auto-Scaling etc
- Can be analysed with the native Metrics Explorer and compared or visualised in an Azure Dashboard or use a Workbook for more complex reporting needs
- Metrics can be streamed to alternate storage mediums such as a Log Analytics Workspace, or accessed over a REST API, CLI or using Powershell commandlets, the former presenting the opportunity for long term trend analysis
- Can archive data for long terms storage for compliance, offline reporting or auditing
- Supports collection of custom application metrics through Application Insights with up to 10 dimensions
- Retains most metrics for up to 93 days but can store some for as long as 2 years
- Natively supports the Log Analytics Agent, Windows Diagnostic Extension (WAD) and Linux Diagnostic Extension (LAD) for collection of guest OS performance counters

### Tracing

Instrumentation for our apps will follow the [OpenTelemetry](https://opentelemetry.io/) API and will be consumed by [Azure Application Insights](https://docs.microsoft.com/en-us/azure/azure-monitor/app/distributed-tracing).

### Logging

Azure Monitor Logs pulls in logs via its Metrics API, meaning:

- We can use Log Analytics in the Azure portal to write log queries and interactively analyze log data.
- We can use the Application Insights analytics console in the Azure portal to write log queries and interactively analyze log data from Application Insights.
- Azure Monitor Logs supports complex data structures

### Alerting

Alerts will be configured through Azure Monitor.

Azure uses the Kusto query language. An example can be found [here](https://github.com/MHRA/products/blob/d609203a5126bdb1ab9bcf1e5d9f910b49231ca1/infrastructure/modules/cluster/alerts.tf#L29).

Action Groups can be associated with alerts to handle SMS / email notifications for people on support duty.

### Visualisation

Azure Dashboard offers basic functionality that is believed to be sufficient for our needs.  Workbooks are an option for more complex usage, should it arise.

## Consequences

No particular risks at this stage to mitigate from our above choices. Pricing for Azure Monitor can be found [here](https://azure.microsoft.com/en-gb/pricing/details/monitor/).