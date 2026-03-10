# Hyper-V Management Pack Extensions

This Hyper-V Management Pack Extensions package is intended to add enhanced performance monitoring to the existing Hyper-V SCOM Management Pack.

This Management Pack includes monitors, rules, views, and dashboards that provide improved visibility into Hyper-V hosts and virtual machines. To avoid excessive database growth, most performance collection rules are disabled by default. These rules can be enabled selectively when needed for environment baselining and deeper analysis.

Monitors are enabled and ready to run in your SCOM environment.

The configured monitor thresholds are designed to cover the most common scenarios, but you may need to tune them to match the specific requirements of your environment.

This Management Pack is free to use and provided to the community. It is delivered as-is, without any support or warranty from Microsoft or GripMatix.

## New features and quality updates
### Release 3.0.0.40
- Support for Windows Server 2019 Hyper-V
- Minor code optimizations

### Release 3.0.0.41
Added the following Performance Rules on Hyper-V Host level:
- Hyper-V MPE 2019 Root Virtual Processor % Total Run Time
- Hyper-V MPE 2019 Root Virtual Processor % Hypervisor Run Time
- Hyper-V MPE 2019 Root Virtual Processor % Guest Run Time
- Hyper-V MPE 2019 Virtual Processor % Guest Run Time
- Hyper-V MPE 2019 Virtual Processor % Hypervisor Run Time
- Hyper-V MPE 2019 Virtual Processor % Total Run Time
- Hyper-V MPE 2019 Logical Processor % Total Run Time
- Hyper-V MPE 2019 Logical Processor % Hypervisor Run Time
- Hyper-V MPE 2019 Logical Processor % Guest Run Time
- Hyper-V MPE 2019 Dynamic Memory Balancer Available Memory (MBytes)
- Hyper-V MPE 2019 Dynamic Memory Balancer Average Pressure (%)

Added the following Performance Rules on Hyper-V VM level:
- Hyper-V MPE 2019 Dynamic Memory VM Average Pressure (%)

Added the following Performance Rules on Hyper-V Logical Processor level:
- Hyper-V MPE 2019 % Guest Run Time

Added the following Performance Rules on Hyper-V Virtual Processor level:
- Hyper-V MPE 2019 Virtual Processor % Total Run Time
- Hyper-V MPE 2019 Virtual Processor % Hypervisor Run Time

- Minor textual optimizations

### Release 4.0.0.0
- Added support for Windows Server Hyper-V 2022 (validated compatibility)
- Added support for Windows Server Hyper-V 2025 (validated compatibility)
- Added new dashboards for Hyper-V Hosts
- Added new dashboards for Hyper-V Virtual Machines
- General enhancements and optimizations
- Updated and extended community edition maintained by GripMatix

## Requirements
- SCOM 2019 Operations Manager or higher

## Required Management Packs
- Microsoft System Center 2019 Management Pack for Hyper-V v11.0.1.0 or higher:  
  https://www.microsoft.com/en-us/download/details.aspx?id=101312

- Microsoft System Center Management Pack for Windows Server Operating System 2016 and 1709 Plus v10.1.0.2 or higher:  
  https://www.microsoft.com/en-us/download/details.aspx?id=54303

- Microsoft System Center Management Pack for Windows Server Cluster 2016 and 1709 Plus v10.1.0.0 or higher:  
  https://www.microsoft.com/en-us/download/details.aspx?id=54701

## Credits
Initial release was based on Hyper-V Management Pack Extensions 2016:  
https://github.com/dmrellan/Hyper-V-Management-Pack-Extensions-2016

It was later extended for Hyper-V 2019 and additional performance rules by Merijn Overgaauw from GripMatix:  
https://github.com/merijnovergaauw/Hyper-V-Management-Pack-Extensions-2019

This version further enhances that work with support for Hyper-V 2022 and 2025, plus new dashboards for Hyper-V Hosts and Virtual Machines.

## Important!
The management pack file names have changed in version 4.0.0.0. The new files cannot be imported over those from previous versions.
Remove the existing management pack files from your SCOM Management Group before importing version 4.0.0.0.

By default, all performance collection rules are disabled. You can enable them manually or import the “Enable All Rules” override Management Pack to enable them all at once.


