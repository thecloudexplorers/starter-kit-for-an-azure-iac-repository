# Src structure

This is the primary directory for all types of source files. The sources are
categorized into three main subdirectories:

📂 iac (Infrastructure as Code): This directory contains a structured folder
hierarchy for managing Infrastructure as Code templates, such as ARM, Terraform,
and Bicep\
📂 Policies: This directory is home to all policy and initiative definitions.\
📂 Params: This directory stores configuration and parameter files without
sensitive information, such as usernames, passwords, and secrets.\
📂 params (Parameters): In this folder, you'll find all parameter files needed
for specific processes and configurations.\
📂 scripts: The "scripts" directory is organized with a folder structure
designed for the effective management of PowerShell scripts.

Example:

```html
📦src
 ┣ 📂iac
 ┣ 📂policy-definitions
 ┣ 📂params
 ┣ 📂scripts
 ┗ 📜readme.md
 ```
