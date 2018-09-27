# OAC Profile

The Profile JSON file can be used to configure psm

Usage

```
psm setup -c Profile.json
``` 

## JSON Fields Description

| Field | Description | Example Values |
| --- | --- | --- |
| username | OAC Username | a@b.com |
| passoword | OAC Password | MyPWD123 |
| identityDomain | Oracle Identity Domain | mycompany |
| region | Oracle Region | emea/us/... |
| outputFormat | PSM Commands output format | json/short/html |
| clientID | OAuth Client Id (Null if no OAuth) | abc |
| clientSecret | OAuth Client Secret (Null if no OAuth) | a123 | 

If No OAuth is needed the whole `OAuth` section must be omitted
