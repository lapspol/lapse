# Windows LAPS

Download the latest version from Releases:       
https://github.com/admpack/Windows-LAPS/releases/tag/3.0

## System requirements

* Requires .NET Framework version 4.6 or higher
* Minimum supported operating systems: Windows Vista or Windows Server 2008

## Introduction

For environments where users must log on to computers without domain credentials, managing passwords can become a challenging task. Such setups significantly increase the risk of a Pass-the-Hash (PtH) credential replay attack. The Local Administrator Password Solution (LAPS) addresses the problem of using a shared local account with the same password across all computers in a domain. LAPS solves this by assigning a unique, randomly generated password to the common local administrator account on each domain computer. Domain administrators can then control which users, such as helpdesk staff, are permitted to read these passwords.

LAPS streamlines password management while enabling organizations to implement recommended cybersecurity practices. Specifically, the solution reduces the risk of lateral movement that occurs when the same local administrative account and password are used on multiple computers. Passwords for each computer’s local administrator account are stored in Active Directory within a protected attribute of the corresponding computer object. Each computer is able to update its own password in Active Directory, while domain administrators can provide read access to authorized users or groups, such as workstation helpdesk administrators.

With LAPS, you can automatically manage local administrator passwords on domain-joined computers so that each password is unique, randomly generated, and securely maintained in the Active Directory environment. The solution relies entirely on Active Directory infrastructure and does not need additional supporting technologies. LAPS utilizes a Group Policy client-side extension (CSE) installed on managed computers to handle all management tasks. Its management tools enable straightforward configuration and administration.
