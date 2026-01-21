# Struktura

V souboru zpracování otázek jsou nejasná nebo neudělaná místa označena "TODO:"

VSCode má built in markdown preview
Používám markdownlint na linting s tímto presetem v settings.json (přijde mi to čitelnější bez preview)

```json
    "markdownlint.config": {
        "MD007": { "indent": 4 },
        "blanks-around-lists": false,
        "blanks-around-headings": { 
            "lines_above": [2, 3, 1, 1, 1, 1],
            "lines_below": [1, 1, 0, 0, 0, 0]
        },
        "no-multiple-blanks": { "maximum": 3 },
    },
```

Na konci mám v plánu celý soubor vyexportovat do pdf
