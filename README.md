# Battle Tracker Content

This repo contains content translations for the [Warcry Unofficial Battle Tracker](https://tracker.warcryunofficial.com).

Several people have asked for and/or offered help with translating the app into their language — now is your chance!

It is not necessary to translate everything at once. I am really hoping we can get this thing together as a community. Don't feel like you need to take on a huge task and go through everything. Every translation helps, even if it is just a single card!

:sparkles: **All contributors will be properly credited in the app!**

## Contributing

If you're comfortable with (or willing to learn) the [GitHub forking workflow](https://guides.github.com/activities/forking/), make all your changes as usual and submit a PR.

Otherwise, you can use GitHub's edit feature to translate files one by one. [A guide is available here](https://help.github.com/en/github/managing-files-in-a-repository/editing-files-in-your-repository).

:warning: Before you jump into translations, **read the "Translating" section below** to avoid any unnecessary confusion.

## Translating

Whichever way you choose to go about contributing, making the translations is easy. Open the file you want to translate and edit it until you're satisfied.

Couple of pointers:

- Use the terminology as it is used in the official materials.
- Use an [imperative](https://en.wikipedia.org/wiki/Imperative_mood) in the card titles (eg. "Deploy Reserves"). The idea is that people who are already a bit familiar with the game can just read the titles as a kind of todo list and they'll know what's up.
- Use passive voice in the card body (eg. "Players deploy any battle groups marked..."). Given that these are rule explanations, it is beneficial to follow this form so that readers are clear who is the subject of each instruction.
- Double check that page references match between the step content and the relevant source material in your language.
- Try to avoid translations that could be confusing in other variants of your language.
- Once you're done with the translation, change the line that reads `translated: false` to `translated: true`.
- Do not translate template variables (words that are in all caps and surrounded by curly braces — eg. `{ROUND}`). These change dynamically based on where they player is in the game and need to stay exactly like this.
- Do not rename front-matter propety keys (the things that start at every line between the two `---` and that end with a colon — eg. `title:`, `section:`, etc..), but **do** translate their value (the stuff _after_ the colon, see example below).
- Do not rename file names.

### Example

Let's say I choose to translate the file [`content/es/deploy-reserves.md`](./content/es/deploy-reserves.md). I open it on GitHub or in my editor and see this:

```
---
section: Battle Round {ROUND} / Reserves Phase
title: Deploy Reserves
subtitle: (if deployment card specifies)
ref: Reserve Phase (Core Book, p.39)
translated: false
---

Starting with the player who has the initiative, players deploy any battle groups marked RND{ROUND}.
```

I fiddle with it until I am satisfied. A fully translated file should look like this:

```
---
section: Ronda de batalla {ROUND} / Fase de reserva
title: Despliega reservas
subtitle: (si la carta de despliegue lo especifica)
ref: Fase de reserva (Libro básico, p.39)
translated: true
---

Empezando por el jugador que tiene iniciativa, los jugadores despliegan los grupos de batalla marcados con RND{ROUND}.
```

Note that the front-matter property keys (eg. `section`, `title`, `ref`), as well as template variables (eg. `{ROUND}`) have remained unchaged and the `translated` variable has been flipped to `true`. [See this commit](https://github.com/arturmuller/battle-tracker-content/commit/49ffaeabf0fefce24b164649cb8fd08db750265f) for a colourful visualization of the changes.

Everything else has been translated, yay.

Now just save, propose the change, and create a pull request (PR). If you're editing on GitHub, just keep clicking the big green buttons until they stop appearing! (But feel free to include any questions/comments in the PR notes if necessary.)

## Progress

I recommend starting with steps for battles that people use the most: Campaign Battle, Open Battle, Pitched Battle, and Exhibition Battle. The good news is that these share many steps. The below is a complete list of steps that these four battle types are composed of. Each cell links to the correct piece of content here on GitHub, so you can just click and start editing.

The steps below are presented in the order in which they appear in the app (taking into account that it's multiple battle types here...). It should be fairly easy to follow along with the app. Here are links for each of the four battle types for your convenience: [Campaign Battle](https://tracker.warcryunofficial.com/campaign-battle), [Open Battle](https://tracker.warcryunofficial.com/open-battle), [Pitched Battle](https://tracker.warcryunofficial.com/pitched-battle), and [Exhibition Battle](https://tracker.warcryunofficial.com/exhibition-battle).

| Step                          | Spanish                                                                            | French                                                                             | German                                                                             |
| ----------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| muster-warbands-for-narrative | [:grey_exclamation: Not Translated](./content/es/muster-warbands-for-narrative.md) | [:grey_exclamation: Not Translated](./content/fr/muster-warbands-for-narrative.md) | [:grey_exclamation: Not Translated](./content/de/muster-warbands-for-narrative.md) |
| muster-warbands-for-matched   | [:grey_exclamation: Not Translated](./content/es/muster-warbands-for-matched.md)   | [:grey_exclamation: Not Translated](./content/fr/muster-warbands-for-matched.md)   | [:grey_exclamation: Not Translated](./content/de/muster-warbands-for-matched.md)   |
| muster-warbands-for-open      | [:grey_exclamation: Not Translated](./content/es/muster-warbands-for-open.md)      | [:grey_exclamation: Not Translated](./content/fr/muster-warbands-for-open.md)      | [:grey_exclamation: Not Translated](./content/de/muster-warbands-for-open.md)      |
| priority-roll                 | [:grey_exclamation: Not Translated](./content/es/priority-roll.md)                 | [:grey_exclamation: Not Translated](./content/fr/priority-roll.md)                 | [:grey_exclamation: Not Translated](./content/de/priority-roll.md)                 |
| battle-groups                 | [:grey_exclamation: Not Translated](./content/es/battle-groups.md)                 | [:grey_exclamation: Not Translated](./content/fr/battle-groups.md)                 | [:grey_exclamation: Not Translated](./content/de/battle-groups.md)                 |
| use-symmetrical               | [:grey_exclamation: Not Translated](./content/es/use-symmetrical.md)               | [:grey_exclamation: Not Translated](./content/fr/use-symmetrical.md)               | [:grey_exclamation: Not Translated](./content/de/use-symmetrical.md)               |
| deal-battleplan-cards         | [:grey_exclamation: Not Translated](./content/es/deal-battleplan-cards.md)         | [:grey_exclamation: Not Translated](./content/fr/deal-battleplan-cards.md)         | [:grey_exclamation: Not Translated](./content/de/deal-battleplan-cards.md)         |
| deal-terrain-and-twist-cards  | [:grey_exclamation: Not Translated](./content/es/deal-terrain-and-twist-cards.md)  | [:grey_exclamation: Not Translated](./content/fr/deal-terrain-and-twist-cards.md)  | [:grey_exclamation: Not Translated](./content/de/deal-terrain-and-twist-cards.md)  |
| determine-battleplan          | [:grey_exclamation: Not Translated](./content/es/determine-battleplan.md)          | [:grey_exclamation: Not Translated](./content/fr/determine-battleplan.md)          | [:grey_exclamation: Not Translated](./content/de/determine-battleplan.md)          |
| deploy-battle-groups          | [:grey_exclamation: Not Translated](./content/es/deploy-battle-groups.md)          | [:grey_exclamation: Not Translated](./content/fr/deploy-battle-groups.md)          | [:grey_exclamation: Not Translated](./content/de/deploy-battle-groups.md)          |
| resolve-terrain-card          | [:grey_exclamation: Not Translated](./content/es/resolve-terrain-card.md)          | [:grey_exclamation: Not Translated](./content/fr/resolve-terrain-card.md)          | [:grey_exclamation: Not Translated](./content/de/resolve-terrain-card.md)          |
| resolve-victory-card          | [:grey_exclamation: Not Translated](./content/es/resolve-victory-card.md)          | [:grey_exclamation: Not Translated](./content/fr/resolve-victory-card.md)          | [:grey_exclamation: Not Translated](./content/de/resolve-victory-card.md)          |
| resolve-twist-card            | [:grey_exclamation: Not Translated](./content/es/resolve-twist-card.md)            | [:grey_exclamation: Not Translated](./content/fr/resolve-twist-card.md)            | [:grey_exclamation: Not Translated](./content/de/resolve-twist-card.md)            |
| initiative-roll               | [:grey_exclamation: Not Translated](./content/es/initiative-roll.md)               | [:grey_exclamation: Not Translated](./content/fr/initiative-roll.md)               | [:grey_exclamation: Not Translated](./content/de/initiative-roll.md)               |
| wild-dice                     | [:grey_exclamation: Not Translated](./content/es/wild-dice.md)                     | [:grey_exclamation: Not Translated](./content/fr/wild-dice.md)                     | [:grey_exclamation: Not Translated](./content/de/wild-dice.md)                     |
| review-initiative             | [:grey_exclamation: Not Translated](./content/es/review-initiative.md)             | [:grey_exclamation: Not Translated](./content/fr/review-initiative.md)             | [:grey_exclamation: Not Translated](./content/de/review-initiative.md)             |
| deploy-reserves               | [:white_check_mark: Translated](./content/es/deploy-reserves.md)                   | [:grey_exclamation: Not Translated](./content/fr/deploy-reserves.md)               | [:grey_exclamation: Not Translated](./content/de/deploy-reserves.md)               |
| activate-fighters             | [:grey_exclamation: Not Translated](./content/es/activate-fighters.md)             | [:grey_exclamation: Not Translated](./content/fr/activate-fighters.md)             | [:grey_exclamation: Not Translated](./content/de/activate-fighters.md)             |
| round-review                  | [:grey_exclamation: Not Translated](./content/es/round-review.md)                  | [:grey_exclamation: Not Translated](./content/fr/round-review.md)                  | [:grey_exclamation: Not Translated](./content/de/round-review.md)                  |
| glory-points                  | [:grey_exclamation: Not Translated](./content/es/glory-points.md)                  | [:grey_exclamation: Not Translated](./content/fr/glory-points.md)                  | [:grey_exclamation: Not Translated](./content/de/glory-points.md)                  |
| injury-roll                   | [:grey_exclamation: Not Translated](./content/es/injury-roll.md)                   | [:grey_exclamation: Not Translated](./content/fr/injury-roll.md)                   | [:grey_exclamation: Not Translated](./content/de/injury-roll.md)                   |
| destiny-roll                  | [:grey_exclamation: Not Translated](./content/es/destiny-roll.md)                  | [:grey_exclamation: Not Translated](./content/fr/destiny-roll.md)                  | [:grey_exclamation: Not Translated](./content/de/destiny-roll.md)                  |
| manage-roster                 | [:grey_exclamation: Not Translated](./content/es/manage-roster.md)                 | [:grey_exclamation: Not Translated](./content/fr/manage-roster.md)                 | [:grey_exclamation: Not Translated](./content/de/manage-roster.md)                 |
| search-artefacts              | [:grey_exclamation: Not Translated](./content/es/search-artefacts.md)              | [:grey_exclamation: Not Translated](./content/fr/search-artefacts.md)              | [:grey_exclamation: Not Translated](./content/de/search-artefacts.md)              |
| advance-campaign              | [:grey_exclamation: Not Translated](./content/es/advance-campaign.md)              | [:grey_exclamation: Not Translated](./content/fr/advance-campaign.md)              | [:grey_exclamation: Not Translated](./content/de/advance-campaign.md)              |
| earn-artefacts-of-power       | [:grey_exclamation: Not Translated](./content/es/earn-artefacts-of-power.md)       | [:grey_exclamation: Not Translated](./content/fr/earn-artefacts-of-power.md)       | [:grey_exclamation: Not Translated](./content/de/earn-artefacts-of-power.md)       |
| thanks                        | [:grey_exclamation: Not Translated](./content/es/thanks.md)                        | [:grey_exclamation: Not Translated](./content/fr/thanks.md)                        | [:grey_exclamation: Not Translated](./content/de/thanks.md)                        |

## Credits

### English

- [@artmllr](https://www.reddit.com/user/artmllr)

### Spanish

- [@bararito](https://github.com/Bararito)

### French

_(No one yet!)_

### German

_(No one yet!)_
