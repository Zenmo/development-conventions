# Abbreviation

Do not abbreviate words in class, method or variable names unless the abbreviation is more common than the full word. This also goes for CSS class names.

Avoid single-letter variable names.

2-letter abbreviations are almost always nonobvious and should be avoided. Never cut off words in names to save space.

Good abbreviations:

- HTTP
- JSON
- ESDL
- CAPEX
- OPEX
- kWh
- kW

Bad abbreviations:

- DA -> Day Ahead
- Conf -> config / configuration

## Variable name exemptions

You **may** use single-letter variables in these cases:

### One-line lambdas

```java
var assetIds = assets.map(a -> a.id)
```

### Loop counters

```java
for (let i = 0; i < assets.length; i++) {
```

## Other exemptions

Common patterns such at T or E for a generic type, or I-prefix for an interface.

# Compound names

Use compound names to clarify meaning and intent.

Good examples:

- rootAsset
- defaultSetting
