# Struktura

V souboru zpracování otázek jsou nejasná nebo neudělaná místa označena ``- [ ] {note}`` a hotová ``- [x] {note}``
- [ ] {note}
- [x] {note}


## Chci se držet této struktury (feel free to recommend something better)

```markdown
---

## Prezentace xy

### **Téma**
- něco k tématu
    - poznámka k něčemu

---
```

### Výsledek

---


## Prezentace xy

### **Téma**
- něco k tématu
    - poznámka k něčemu

---


VSCode má built in markdown preview a pro editing používám [Markdown All in One](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one), který má normální klávesové zkratky a QoL improvements.
Používám markdownlint na linting s tímto presetem v settings.json

```json
    "markdownlint.config": {
        "MD007": { "indent": 4 },
        "blanks-around-lists": false,
        "blanks-around-headings": { 
            "lines_above": [2, 2, 1, 1, 1, 1],
            "lines_below": [1, 1, 0, 0, 0, 0]
        },
        "no-multiple-blanks": { "maximum": 3 },
    },
```


Na konci mám v plánu celý soubor vyexportovat do pdf
