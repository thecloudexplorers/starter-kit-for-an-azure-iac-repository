# Purpose

This folder contains IaC files that are used as a unit of code reuse. A module
can contain a single resource or set of resources, and can be called
from controllers. This allows deployments to be small, manageable components,
and reuse common pieces.

For the purposes of traceability and discoverability, each module is organized
in a folder structure that aligns with the [Azure Resource Provider](https://learn.microsoft.com/en-us/azure/azure-resource-manager/management/resource-providers-and-types)
structure. An additional advantage of this approach is that the required
`Azure Resource Providers` are immediately visible. Furthermore, automation can
be established to manage any drift in the providers, based on the modules.\
The module folder contains two subfolders: `samples` and `test`. The `samples`
folder contains a script and if required configuration that can be used to
deploy the module locally. The `test` folder contains all the test related
materials. For example a unit test and scenario specific parameter files that
can be used to test the module. In addition the folder contains a `readme.md`
file that describes the module and its usage.
The module itself is typically named deploy but can be named differently.

Example structure:

```html
📦az-modules
 ┣ 📂Microsoft.Authorization
 ┃ ┗ 📂policyassignments
 ┃   ┣ 📂samples
 ┃   ┃ ┗ localDeploy.ps1
 ┃   ┣ 📂test
 ┃   ┃ ┣ happy-flow.params.json
 ┃   ┃ ┣ invalid-setting.params.json
 ┃   ┃ ┗ unhappy-flow.params.json
 ┃   ┣ deploy.bicep
 ┃   ┗ 📜readme.md
 ┣ 📂Microsoft.KeyVault
 ┃ ┗ 📂vaults
 ┃   ┣ 📂samples
 ┃   ┃ ┗ localDeploy.ps1
 ┃   ┣ 📂test
 ┃   ┃ ┣ happy-flow.params.json
 ┃   ┃ ┣ invalid-setting.params.json
 ┃   ┃ ┗ unhappy-flow.params.json
 ┃   ┣ deploy.bicep
 ┃   ┗ 📜readme.md
 ┣ 📂Microsoft.Network
 ┃ ┣ 📂dnszones
 ┃ ┃ ┣ 📂samples
 ┃ ┃ ┃ ┗ localDeploy.ps1
 ┃ ┃ ┣ 📂test
 ┃ ┃ ┃ ┣ happy-flow.params.json
 ┃ ┃ ┃ ┣ invalid-setting.params.json
 ┃ ┃ ┃ ┗ unhappy-flow.params.json
 ┃ ┃ ┣ deploy.bicep
 ┃ ┃ ┗ 📜readme.md
 ┃ ┗ 📂virtualnetworks
 ┃   ┣ 📂samples
 ┃   ┃ ┗ localDeploy.ps1
 ┃   ┣ 📂test
 ┃   ┃ ┣ happy-flow.params.json
 ┃   ┃ ┣ invalid-setting.params.json
 ┃   ┃ ┗ unhappy-flow.params.json
 ┃   ┣ deploy.bicep
 ┃   ┗ 📜readme.md
 ┣ 📂Microsoft.Storage
 ┃ ┗ 📂storageaccounts
 ┃   ┣ 📂samples
 ┃   ┃ ┗ localDeploy.ps1
 ┃   ┣ 📂test
 ┃   ┃ ┣ happy-flow.params.json
 ┃   ┃ ┣ invalid-setting.params.json
 ┃   ┃ ┗ unhappy-flow.params.json
 ┃   ┣ deploy.bicep
 ┃   ┗ 📜readme.md
 ┗ 📜readme.md
```
