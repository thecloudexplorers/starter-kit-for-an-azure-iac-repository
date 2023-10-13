# Pipelines structure

All pipelines must be placed within this folder. For each individual pipeline,
create a corresponding subfolder. Please adhere to the following structural
rules:

- Each pipeline should have its own dedicated folder.
- Depending on the design of the pipeline, you can choose between two options:
  - A single `📜.yml` file that contains all the required stages.
  - Multiple `📜.yml` files to represent different stages of the pipeline.
- In addition, each pipeline folder must include a `📜readme.md` file that
  contains technical documentation elucidating the specifics of the respective
  pipeline.

By following these guidelines, you can maintain an organized and well-documented
approach to managing pipelines.

Example:

```html
📦 pipelines
 ┣ 📂 management
 ┃ ┣ 📄 managementStructure.yml
 ┃ ┗ 📄 readme.md
 ┣ 📂 workload
 ┃ ┣ 📄 deploy-workload.yml
 ┃ ┗ 📄 readme.md
 ┣ 📂 microservice-deploy
 ┃ ┣ 📄 deploy-microservice.yml
 ┃ ┗ 📄 readme.md
 ┗ 📄 readme.md

```
