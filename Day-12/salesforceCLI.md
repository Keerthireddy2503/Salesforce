## Salesforce CLI Tutorial

### Focus: Command-Line Workflow

The Salesforce CLI (Command Line Interface) is a tool that lets developers work with Salesforce directly from the terminal instead of using only the browser UI. It helps automate development tasks and speeds up workflow. ([Salesforce Ben][1])

---

## What You Learn in the Tutorial

### 1. Command-Line Basics

CLI commands follow this structure:

```bash
sf command flags arguments
```

Example:

```bash
sf project generate --name MyProject
```

Parts:

* **Command** → action to perform
* **Flag** → extra option (`--name`)
* **Argument** → value (`MyProject`) ([Trailhead][2])

---

## 2. Common Salesforce CLI Workflow

### Login to Salesforce Org

```bash
sf org login web
```

Opens browser login and connects your org.

---

### Create Salesforce Project

```bash
sf project generate --name FirstProject
```

Creates a new Salesforce DX project folder.

---

### Open Project in VS Code

```bash
code .
```

Opens current folder in [Visual Studio Code](https://code.visualstudio.com?utm_source=chatgpt.com)

---

### Retrieve Metadata

```bash
sf project retrieve start
```

Pulls metadata from Salesforce org to local machine.

---

### Deploy Changes

```bash
sf project deploy start
```

Pushes local code/metadata to org. ([Developer][3])

---

### Run Apex Tests

```bash
sf apex run test
```

Executes Apex test classes.

---

## 3. Navigation Commands

| Command         | Purpose          |
| --------------- | ---------------- |
| `cd folderName` | Move into folder |
| `mkdir folder`  | Create folder    |
| `dir` / `ls`    | View files       |
| `code .`        | Open VS Code     |

These are basic terminal commands used daily in CLI workflows. ([Trailhead][2])

---

## 4. Salesforce CLI Advantages

* Faster development
* Automation support
* Easier deployments
* Better DevOps workflow
* GitHub integration
* Supports CI/CD pipelines

Salesforce CLI is considered a core tool in modern Salesforce DX development. ([Developer][4])

---

## 5. Important Modern Commands

Salesforce now mainly uses `sf` commands instead of older `sfdx` commands.

Example:

```bash
sf org list
sf project deploy start
sf apex generate class
```

The newer `sf` CLI is cleaner and more organized. ([Developer][4])

---

## Beginner Practice Flow

```text
Install Salesforce CLI
        ↓
Create Project
        ↓
Login to Org
        ↓
Retrieve Metadata
        ↓
Edit in VS Code
        ↓
Deploy Changes
        ↓
Run Tests
[3]: https://developer.salesforce.com/docs/platform/salesforce-cli-plugin/guide/common-actions.html?utm_source=chatgpt.com "Common Actions | Design Principles and Guidelines | Salesforce CLI Plugin Developer Guide | Salesforce Developers"
[4]: https://developer.salesforce.com/blogs/2023/07/the-salesforce-cli-sf-v2-is-here-part-2?utm_source=chatgpt.com "The Salesforce CLI sf (v2) Is Here! — Part 2 | Salesforce Developers Blog"
