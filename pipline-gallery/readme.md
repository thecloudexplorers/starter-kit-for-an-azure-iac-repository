# Purpose

The pipeline gallery is intended for housing reusable pipeline components like
jobs, and steps. For consistency jobs and steps should be stored
separate folders.

Example structure:

```html
📦pipeline-gallery
 ┣ 📂jobs
 ┃ ┣ 📜deploySolution.yml
 ┃ ┣ 📜deployInfrastructure.yml
 ┃ ┣ 📜staticAnalysis.yml
 ┃ ┗ 📜codeQualityValidation.yml
 ┣ 📂steps
 ┃ ┣ 📜buildSolution.yml
 ┃ ┣ 📜staticAnalysis.yml
 ┃ ┣ 📜publishSolutionArtifacts.yml
 ┃ ┗ 📜buildBicep.yml
 ┗ 📜readme.md
```
