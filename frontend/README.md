Frontend development conventions
===

Zenmo follows the general trend in frontend development: a component-based approach and no CSS preprocessing.

We use the default style of prettier, with the following customization:

```javascript
export default {
    // 4-space indent
    tabWidth: 4,
    // No semicolons
    semi: false,
    // && and || at the start of the line
    experimentalOperatorPosition: "start",
}
```
