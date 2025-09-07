---
tags:
  - plugin
resource_link: "https://www.redguides.com/community/resources/mq2bandolier.101/"
support_link: "https://www.redguides.com/community/threads/mq2bandolier.66806/"
repository: "https://github.com/RedGuides/MQ2Bandolier"
config: "MQ2Bandolier_character.ini"
authors: "Wassup, Woobs, Knightly"
tagline: "Extends the functionality of EQ's Bandolier, allowing you to change items in any slot."
quick_start: "https://www.redguides.com/wiki/MQ2Bandolier#Simple_Setup"
---

# MQ2Bandolier
<!--desc-start-->
While EverQuest's built-in [/bandolier](../everquest/commands/cmd-bandolier.md) allows you to exchange weapons, MQ2Bandolier goes a step further and gives you the ability to swap out any slot, it can even exchange entire suits of armor. Requires [MQ2Exchange](../mq2exchange/index.md) to function.
<!--desc-end-->

## Commands

<a href="cmd-createset/">
{% 
  include-markdown "projects/mq2bandolier/cmd-createset.md" 
  start="<!--cmd-syntax-start-->" 
  end="<!--cmd-syntax-end-->" 
%}
</a>
:    {% include-markdown "projects/mq2bandolier/cmd-createset.md" 
        start="<!--cmd-desc-start-->" 
        end="<!--cmd-desc-end-->" 
        trailing-newlines=false 
     %} {{ readMore('projects/mq2bandolier/cmd-createset.md') }}

<a href="cmd-deleteset/">
{% 
  include-markdown "projects/mq2bandolier/cmd-deleteset.md" 
  start="<!--cmd-syntax-start-->" 
  end="<!--cmd-syntax-end-->" 
%}
</a>
:    {% include-markdown "projects/mq2bandolier/cmd-deleteset.md" 
        start="<!--cmd-desc-start-->" 
        end="<!--cmd-desc-end-->" 
        trailing-newlines=false 
     %} {{ readMore('projects/mq2bandolier/cmd-deleteset.md') }}

<a href="cmd-equipset/">
{% 
  include-markdown "projects/mq2bandolier/cmd-equipset.md" 
  start="<!--cmd-syntax-start-->" 
  end="<!--cmd-syntax-end-->" 
%}
</a>
:    {% include-markdown "projects/mq2bandolier/cmd-equipset.md" 
        start="<!--cmd-desc-start-->" 
        end="<!--cmd-desc-end-->" 
        trailing-newlines=false 
     %} {{ readMore('projects/mq2bandolier/cmd-equipset.md') }}

## Settings

When editing the MQ2Bandolier_character.ini, only slot numbers are used. Here are the slots they correspond to:

### Equipment slots:
{% 
  include-markdown "projects/macroquest/reference/general/slot-names.md" 
  start="### Equipment Slots" 
  end="### Inventory Slots" 
%}

### Inventory slots:
{% 
  include-markdown "projects/macroquest/reference/general/slot-names.md" 
  start="### Inventory Slots" 
  end="### Bank Slots" 
%}

See [Slot names](../macroquest/reference/general/slot-names.md) for more slot names.

When creating a set in-game via */createset*, you may use slot names, but they will be saved to the .ini as slot numbers. For example,

```bash
/createset watergear leftfinger back
```

and 

```ini
/createset landgear 15 8
```

will be saved in your MQ2Bandolier_character.ini as,

```ini
[water]
15=30070
8=22816
[land]
15=25198
8=15840
```

The numbers after the slot number correspond to the item ID. These are automatically generated.

## Simple Setup

Put on your wedding gear and type,

```bash
/createset WeddingDay head chest legs arms
```

Now you can look great instantly when you type this command:

```bash
/equipset WeddingDay
```

## See also

- [MQ2Exchange](../mq2exchange/index.md)
- [Slot names](../macroquest/reference/general/slot-names.md)
- [/bandolier](../everquest/commands/cmd-bandolier.md)
