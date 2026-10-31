# D&D Action Sheet

A simple, single-file action tracker for your Dungeons & Dragons character. Keep every action, bonus action, reaction and limited-use ability in one place, track uses between rests, and print or export your sheet.

> **Disclaimer:** This project was created with the help of AI.

## Features

- Add any action your character can take: attacks, spells, class features, racial traits, feats and item abilities
- Sorted by action type: Action, Bonus Action, Reaction, Free Action, Movement, Other
- Prefilled with the standard actions (Attack, Dash, Disengage, Dodge, Help, Hide, Ready, Opportunity Attack)
- Clickable use counters for limited abilities, with Short Rest and Long Rest buttons
- Search and filter tabs
- Compact print layout (several actions per page)
- Export as JSON backup or Markdown list, and import a backup again
- Dark theme (black and grey with purple accents)
- No installation, no server, no accounts, no tracking

## Quick start

1. Download `index.html`.
2. Open it in any modern browser (Chrome, Firefox, Safari, Edge).
3. Start adding actions.

That's it. The whole app is one HTML file with no external dependencies.

Or

1. Open https://ertreuer.github.io/DnD-5e-Action-Sheet/ and start with How to use

## How to use

### Add an action

1. Click **+ New action**.
2. Fill in the form:
   - **Name**: e.g. *Fireball* or *Second Wind*
   - **Action type**: Action, Bonus Action, Reaction, Free Action, Movement or Other
   - **Source**: General, Class, Race, Spell, Feat, Item or Weapon
   - **Range / duration**: e.g. *60 ft, concentration*
   - **Attack / saving throw**: e.g. *+7* or *DEX save DC 15*
   - **Damage / effect**: e.g. *8d6 fire*
   - **Uses**: how many times per rest (0 means unlimited)
   - **Recharges on**: Short rest, Long rest, or nothing
   - **Description / notes**: anything you want to remember
3. Click **Save**.

### Track limited uses

Abilities with a number of uses show round counters on their card.

- Click a counter to mark a use as spent. Click it again to give the use back.
- **Short Rest** restores everything set to recharge on a short rest.
- **Long Rest** restores everything set to recharge on a short or long rest.

### Find things fast

- Use the **tabs** to show only one action type (the number shows how many entries it has).
- Use the **search box** to filter by name, description or source.

### Edit or delete

Every card has **Edit** and **Delete** buttons. This includes the prefilled standard actions, so remove anything you don't need.

### Print

Click **Print**. The print view always shows all actions, in two compact columns, without buttons or tabs. In the print dialog you can switch to a different paper size or save as PDF.

### Export and import

- **Export backup (JSON)** saves your full sheet to a file. Use this to back up your character or move it to another device.
- **Export list (Markdown)** saves a readable list grouped by action type, handy for notes apps or Discord.
- **Import backup** loads a JSON backup. It replaces your current sheet after you confirm.

Tip: give your sheet a character name at the top. It is used for the print title and the export file names.

## Your data

Everything is stored in your browser's local storage on your own device. Nothing is sent anywhere.

- Each person (and each browser) has their own sheet.
- Clearing your browser data deletes your sheet, so export a backup now and then.
- To use the same sheet on another device, export a JSON backup and import it there.
- To share a ready-made character with a friend, send them your JSON file.

## Hosting it for free

Because it's a single static file, you can host it almost anywhere:

- **GitHub Pages**: upload `index.html` to a repository, then go to *Settings → Pages* and select your main branch.
- **Netlify Drop**: drag the file onto [app.netlify.com/drop](https://app.netlify.com/drop).
- **Cloudflare Pages** or any other static host works too.

Share the link with your party. Everyone gets their own private sheet.

## Customizing

All colors are defined as CSS variables at the top of `index.html` (`--bg`, `--card`, `--acc`, and so on), so you can change the theme in a few lines. Default action types and sources are plain `<option>` lists in the form and can be edited directly.

## Disclaimer

This project was created with the help of AI. It is an unofficial fan tool and is not affiliated with or endorsed by Wizards of the Coast. Dungeons & Dragons is a trademark of Wizards of the Coast LLC. Please check rules and numbers against your official sources.
