## LWC Communication Explained


### Focus

* Parent-child communication
* Events
* Component interaction

---

# Types of Communication in LWC

```text
1. Parent → Child
2. Child → Parent
3. Unrelated Components
```

LWC mainly uses `@api`, events, and Lightning Message Service for communication. ([Akhil Kulkarni][1])

---

# 1. Parent to Child Communication

Parent sends data using `@api`.

### Child JS

```javascript
@api message;
```

### Parent HTML

```html
<c-child message="Hello"></c-child>
```

`@api` makes child properties public. ([Akhil Kulkarni][1])

---

# 2. Child to Parent Communication

Child sends data using custom events.

### Child JS

```javascript
this.dispatchEvent(
    new CustomEvent('save')
);
```

### Parent HTML

```html
<c-child onsave={handleSave}></c-child>
```

Custom events are the standard way for child-to-parent interaction. ([Akhil Kulkarni][2])

---

# 3. Component Interaction

For unrelated components:

* Lightning Message Service (LMS)
* PubSub

Used when components are not directly connected. ([Akhil Kulkarni][1])

---

# Event Flow

```text
User Action
    ↓
Event Trigger
    ↓
Parent Handles Event
```

Events help components communicate efficiently. ([salesforcebolt.com][3])

---

# Important Concepts

| Concept           | Purpose                          |
| ----------------- | -------------------------------- |
| `@api`            | Public property/method           |
| `CustomEvent`     | Send events                      |
| `dispatchEvent()` | Trigger event                    |
| LMS               | Communicate unrelated components |

---

# Real Example

| Scenario            | Communication Type |
| ------------------- | ------------------ |
| Form data display   | Parent → Child     |
| Button click update | Child → Parent     |
| Dashboard refresh   | LMS                |

