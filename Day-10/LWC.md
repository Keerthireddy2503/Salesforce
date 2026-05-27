## LWC Full Course for Beginners


### Focus

* LWC architecture
* Component structure
* Real examples

---

# What is LWC?

Lightning Web Components (LWC) is Salesforce’s modern UI framework built using:

* HTML
* JavaScript
* CSS

---

# LWC Architecture

```text
LWC Component
 ├── HTML
 ├── JavaScript
 ├── CSS
 └── XML
```

---

# Component Structure

```text
helloWorld/
 ├── helloWorld.html
 ├── helloWorld.js
 ├── helloWorld.js-meta.xml
 └── helloWorld.css
```

---

# Simple Example

### HTML

```html
<template>
    <h1>Hello Salesforce</h1>
</template>
```

### JavaScript

```javascript
import { LightningElement } from 'lwc';

export default class HelloWorld extends LightningElement {}
```

---

# Create LWC Component

```bash
sf lightning generate component --name helloWorld
```

Deploy:

```bash
sf project deploy start
```

---

# Real Examples

| Example          | Purpose              |
| ---------------- | -------------------- |
| Contact Card     | Display records      |
| To-Do App        | Event handling       |
| Search Component | Search/filter data   |
| Account Table    | Show Salesforce data |

---

# Important Concepts

* `@api` → Public property
* `@wire` → Fetch Salesforce data
* `@track` → Track changes

Example:

```javascript
@api recordId;
```

---

# Advantages of LWC

* Fast performance
* Reusable components
* Modern JavaScript
* Easy maintenance
* Mobile friendly

---

# Learning Flow

```text
HTML/CSS
   ↓
JavaScript
   ↓
LWC Basics
   ↓
Events & Data
   ↓
Apex Integration
```

---

