# Battle Tracker Content

This repo contains content translations for the [Warcry Unofficial Battle Tracker](https://tracker.warcryunofficial.com).

## Contributing

If you're comfortable with (or willing to learn) the [GitHub forking workflow](https://guides.github.com/activities/forking/), simply make all your desired changes as outlined below and then open a PR.

Otherwise, you can use GitHub's edit feature to translate files one by one. [A guide is available here](https://help.github.com/en/github/managing-files-in-a-repository/editing-files-in-your-repository).

## Translating

Whichever way you choose to go about contributing, actually making the translations is easy. Open the file you want to translate and edit it until you're satisfied.

Couple of pointers:

- Use the terminology as it is used in the official materials.
- Try to avoid translations that strongly hint at your regional variant of the language.
- Double check that page references match between the step content and the relevant source material in your language.
- Once you're done with the translation, change the line that reads `translated: false` to `translated: true`.
- Do not translate template variables (words that are in all caps and surrounded by curly braces — eg. `{ROUND}`). These change dynamically based on where they player is in the game and need to stay exactly like this.
- Do not rename front-matter propety keys (the things that start at every line between the two `---` — eg. `title:`, `section`, etc..), but **do** translate their value (see example below if you're unsure).
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

I fiddle around it until I am satisfied. A fully translated file should look like this:

```
---
section: Battle Round {ROUND} / Reserves Phase
title: Deploy Reserves
subtitle: (if deployment card specifies)
ref: Fase de reserva (Libro Básico, p.39)
translated: true
---

XXX RND{ROUND}.
```

Note that the front-matter property keys (eg. `section`, `title`, `ref`), as well as template variables (eg. `{ROUND}`) have remained unchaged and the `translate` variable has been flipped to `true`.

Everything else has been transated, yay.

Now just save and propose the change.

## Credits

### English

- [@artmllr](https://www.reddit.com/user/artmllr)

### Spanish

_(No one yet!)_

### French

_(No one yet!)_
