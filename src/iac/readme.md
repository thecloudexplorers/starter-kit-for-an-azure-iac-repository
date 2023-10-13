# Purpose

The main folder for any Infrastructure as Code files. As best practices dictate
these are divided into two categories: modules and controllers.

## Module

These are essentially Bicep files that are used as a unit of code reuse. A
module can encapsulate a single resource or set of resources, and can be called
from controllers. This allows you to break down deployments into smaller, more
manageable components, and reuse common pieces.

## Controllers

These are Infrastructure as Code files which are used to orchestrate or control
the deployment of various modules. Determining the order in which modules are
deployed, passing parameters to the modules, and handling any dependencies
between modules.

Example structure:

```html
📦iac
 ┣ 📂az-controllers
 ┃ ┣ 📂subscription-vending
 ┃ ┣ 📂compliance-policies
 ┃ ┗ 📂defender-plans
 ┣ 📂az-modules
 ┃ ┣ 📂Microsoft.Authorization
 ┃ ┣ 📂Microsoft.KeyVault
 ┃ ┣ 📂Microsoft.Network
 ┃ ┗ 📂Microsoft.Storage
 ┗ 📜readme.md
```
