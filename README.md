Timetracker REST API Sample Code
===================

This repo contains code samples for using the REST API's in Timetracker. The code is optimized to be simple and easy to understand.

The OData Connected Service Extension (https://docs.microsoft.com/en-us/odata/client/code-generation-tool) has been used to build this code sample.

Reporting API Overview documentation: https://support.7pace.com/hc/en-us/articles/360035502332-Reporting-API-Overview

## TimetrackerReportingClient usage

This is a sample of the console application which connects to DevOps (former VSTS) or DevOps Server (On-premise, former TFS) version of Timetracker and returns all work items with time records for last 3 months.
Command line parameters:

DevOps usage (token auth): 
```
TimetrackerReportingClient.exe ServiceURI -t Token -c System.RemoteLinkCount,System.CommentCount,System.IterationLevel1 -x json

