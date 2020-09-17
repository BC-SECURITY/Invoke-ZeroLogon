# Invoke-ZeroLogon
This code was heavily adapted from the C# implementation by the [NCC Group's Full Spectrum Attack Simulation team](https://github.com/nccgroup/nccfsas/tree/main/Tools/SharpZeroLogon) and the original CVE published by [Secura](https://www.secura.com/blog/zero-logon).
This script can be run in two modes: 
1.	When the reset parameter is set to True, the script will attempt to reset the target computer’s password to the default NTLM hash (essentially an empty password).
2.	By default, reset is set to false and will simply scan if the target computer is vulnerable to the ZeroLogon exploit (CVE-2020-1472).

__WARNING:__ Resetting the password of a Domain Controller is likely to break the network. __DO NOT__ use the reset parameter against a production system unless you fully understand the risks and have explicit permission.
