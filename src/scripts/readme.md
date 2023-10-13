# Purpose

The main folder for any scripts. As best practices dictate scripts are divided
into two categories: functions and controllers.

## Functions

They are essentially small scripts that can perform a specific task and can be
called upon in a larger script (controller), making the code more modular and
easier to manage. They are designed for high level of reusability.

## Controllers

While not all languages implement controllers the term is in a broader sense
applicable to most languages. Controllers are essentially scripts that utilize
one or more tools (functions, commands, etc) to automate a specific business
process. A controller script is not intended to be reusable; it is intended to
make use of reuse by leveraging functions and other commands. Instead
controllers are intended to be rerunnable.

Example:

> NOTE: if multiple languages are used, it is recommended to create a subfolder
> per language.

```html
📦scripts
 ┣ 📂controllers
 ┃ ┣ 📜roleDefinitionsForWorkloads.ps1
 ┃ ┣ 📜subscriptionVending.ps1
 ┃ ┣ 📜policyDefinitions.ps1
 ┃ ┗ 📜roleAssignmentsForWorkloads.ps1
 ┣ 📂functions
 ┃ ┣ 📜New-AzAdApp.ps1
 ┃ ┣ 📜Set-AzRoleAssignment.ps1
 ┃ ┣ 📜New-AdoAuthenticationToken.ps1
 ┃ ┗ 📜Confirm-AdoGroupMembership.ps1
 ┗ 📜readme.md
```
