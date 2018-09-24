# OAC Instance Creation

The Json payload can be used to create an OAC instance (with the related DBCS already UP and Running)

Usage:

```
psm analytics create-service -c OAC.json
```

## JSON Fields Description

| Field | Description | Example Values |
| --- | --- | --- |
| Edition | OAC Edition | EE |
| vmPublicKeyText | OAC SSH Public Key | ssh-rsa `PUBLIC SSH KEY` |
| enableNotification | Enable/Disable Notifications | true/false |
| notificationEmail | OAC Notification Email | email |
| serviceVersion | OAC Service Version | 12.2 |
| isBYOL | IS CUSTOMER BYOL (Bring Your Own License from on-premises) | true/false |
| adminUserName | OAC Administrator Username | Admin |
| adminUserPassword | OAC Administrator Password | MyPWD123 |
| analyticsStorageUser | Analytics Storage User | a@b.com |
| analyticsStoragePassword | Analytics Storage Password | MyPWD123 | 
| shape | Compute Shape | oc1m |
| createAnalyticsStorageContainer | Create a **new** Analytics Storage Container | true/false |
| totalAnalyticsStorage | Total space (in GB) allocated in the newly created Analytics Storage | 280.0 |
| profile_essbase | Include Essbase | true/false |
| profile_bi | Include Answers/Dashboards | true/false |
| profile_dv_forced | Include Data Visualization | true/false |
| dbcsPDBName | Database Cloud Service PDB name to be used to store OAC schemas | PDB1 |
| dbcsUserName | Database Cloud Service Username (with DBA capabilities) | SYS |
| dbcsPassword | Database Cloud Service Password | MyPWD123 |
| dbcsName | Database Cloud Service Instance Name | dbcs1 |
| idcs_enabled | Is Identity Cloud Service enables | true/false |
| analyticsStorageContainerURL | Analytics Storage URL to be used | https://`INSTANCE_NAME`.`AREA`.storage.oraclecloud.com/v1/Storage-`INSTANCE_NAME`/`STORAGE_NAME` |
| publicStorageEnabled | Is public storage enables | true/false |
| usableAnalyticsStorage | Quota of used Analytics Storage | 180 |
| serviceLevel | Service Level | PAAS |
| meteringFrequency | Metering | HOURLY/MONTHLY |
| subscriptionId | Subscription Id | 111111 |
| serviceName | OAC Service Name | OAC



