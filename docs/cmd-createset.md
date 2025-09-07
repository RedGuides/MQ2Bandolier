---
tags:
  - command
---

# /createset

## Syntax

<!--cmd-syntax-start-->
```eqcommand
/createset <setname> slotname1 slotname2 ... (slotname22)
```
<!--cmd-syntax-end-->

## Description

<!--cmd-desc-start-->
Creates an equipment set that's saved to the MQ2Bandolier_character.ini
<!--cmd-desc-end-->

## Options

| Option | Description |
|--------|-------------|
| `setname` | The name of the equipment set. You'll need this when using /equipset |
| `#` or `name` | The slot number OR slot name. The slots are listed on the [settings page](index.md#settings). |

## Examples

Creates a set called "ThisSet" with your equipped chest, main hand and off hand.
```ini
/createset ThisSet chest mainhand offhand
```

The same thing but with numbers instead of names.
```ini
/createset ThisSet 17 13 14
```