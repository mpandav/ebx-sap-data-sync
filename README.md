# Data Sychronisation between EBX and SAP 
A Material Data synchronisation between MDM (EBX) and SAP R3 Systems using TIBCO BusinessWorks

## Pre-requisites
To view or use this application in Businessworks Studio you need to install below prerequitestes.

- TIBCO EMS Server (Transport) or any JMS based transport
- TIBCO BusinessWorks version 6.8 or later or equivalent BWCE version
- SAP Solutions plugin for BusinessWorks

# Architecture
A illustration through block diagram will look like below where we are receiving a New record event from MDM Server (EBX) over JMS Server (TIBCO EMS) as a transport and then using TIBCO BusinessWorks6/CE we are transforming the receiving event into meaningful message by connecting with Master Data System over ReST APIs and then synchronise that Message into SAP R3 System using TIBCO plugin for SAP Solutions. At the end the master record in EBX is getting updated with SAP Material reference ID.

![image](https://github.com/mpandav/ebx-sap-data-sync/assets/38240734/1cdf9729-0d23-4ffc-859c-949d74e01149)


# Demo
A short glimpse of the applciation functionality. 

https://github.com/mpandav/ebx-sap-data-sync/assets/38240734/10ea9eb5-499b-4fc9-97b3-a12010b1eb2b

