# CloudFormation Conditions to update DHCP Options

This repository contains CloudFormation templates that deploy custom VPC DHCP options based on conditions.
There are 2 files:
1. `dchp-resources-conditions-params.yaml` - this template uses a parameter `DHCPWithDomainNameFlag` to determine whether the DHCP option should be created with domain name values. If no, no domain name values will be used in the DHCP Option Set.
2. `dchp-resources-conditions-acctid.yaml` - this template checks the current AWS Account ID to determine whether the DHCP option should be created with domain name values. Note that you would need to update the account IDs listed in `IsDHCPWithDomainName` condition definition.

## Disclaimer

**This project is used for demo purposes only and should NOT be considered for production use.**
