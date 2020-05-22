# Naming conventions
Within Azure, every resource must have a unique name. To help with naming I've come up with a convention using in my project (and this repository).

## Default naming template

**DO** apply the following pattern while naming resources:

``` AAA-BBB-CCC-DDD-EEE ```

| Part | Abbreviation For | Example
| ---- | -----------| ---
| AAA  | Company | CHR (Chroomsoft)
| BBB  | Product | MTA (My Template Abbreviation)
| CCC  | Resource | ASP (App Service Plan)
| DDD  | Stage | DEV, PRD
| EEE  | Location | WE (West Europe)

> *Some Azure resources prevents the use of the above pattern. However try to stay close to this pattern. For example a Azure Storage Account, apply the following pattern: aaabbbcccdddeee*

**AVOID** small letter in the abbreviation.

**CONSIDER** three letter abbreviations for each part of the template. 

**DO** use the abbreviations as specified in the tables below:

**DO NOT** apply this pattern to DNS Zones since they are named after the domain name and are by definition unique. 

## Resource abbreviations
Some of the resources are noted down below:

| Resource           | Abbreviation 
| ------------------ | ---
|App Service Plan|ASP
|Application Insights|AI
|Azure Function App|AFA
|CDN Endpoint|CEN
|CDN Profile|CDN
|Key Vault|KV
|Resource Group|RG
|Shared Dashboard|SDB
|Storage Account|sa
|User managed identity|UMI
|Web site|WEB

## Location abbreviations

| Location      | Abbreviation |
| 