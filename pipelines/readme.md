# Pipelines structure

All pipelines must be placed within this folder. The following set-up is expected for this folder:

- Each pipeline should have its own dedicated folder.
- Depending on the design of the pipeline, you can choose between two options:
  - A single multistage `📜.yml` file that contains all the stages or environments.
  - Multitude of `📜.yml` files to represent each stage or environment.
- Each pipeline folder must include a `📜readme.md` file that contains technical
  documentation elaborating on the specifics of the respective pipeline.

Example structure:

```html
📦 pipelines
 ┣ 📂 management
 ┃ ┣ 📜 managementStructure.yml
 ┃ ┗ 📜 readme.md
 ┣ 📂 workload
 ┃ ┣ 📜 deploy-workload.yml
 ┃ ┗ 📜 readme.md
 ┣ 📂 microservice-deploy
 ┃ ┣ 📜 deploy-microservice.yml
 ┃ ┗ 📜 readme.md
 ┗ 📜 readme.md

```
