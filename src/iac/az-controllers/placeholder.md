# Purpose

This folder contains IaC files that are used as controllers or orchestrators.
Meaning scripts which are intended to utilize one or more modules to deploy
resources.

Each controller is placed in a similar named folder. The folder contains two
subfolders: `samples` and `test`. The `samples` folder contains a script and if
required configuration that can be used to deploy the controller locally. The
`test` folder contains all the test related materials. For example a unit test
and scenario specific parameter files that can be used to test the controller.
In addition the folder contains a `readme.md` file that describes the controller
and its usage.
The module itself is typically named equally to the folder but based on
preference can be named differently.

Example structure:

```html
📦az-controllers
 ┣ 📂defender-plans
 ┃ ┣ 📂samples
 ┃ ┃ ┗ localDeploy.ps1
 ┃ ┣ 📂test
 ┃ ┃ ┣ happy-flow.params.json
 ┃ ┃ ┣ invalid-setting.params.json
 ┃ ┃ ┗ unhappy-flow.params.json
 ┃ ┣ 📜defender-plans.bicep
 ┃ ┗ 📜readme.md
 ┣ 📂subscription-vending
 ┃ ┣ 📂samples
 ┃ ┃ ┗ localDeploy.ps1
 ┃ ┣ 📂test
 ┃ ┃ ┣ happy-flow.params.json
 ┃ ┃ ┣ invalid-setting.params.json
 ┃ ┃ ┗ unhappy-flow.params.json
 ┃ ┣ 📜subscription-vending.bicep
 ┃ ┗ 📜readme.md
 ┗ 📜readme.md
```
