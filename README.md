# Recipes

Each recipe is one file in `_recipes/`. GitHub Pages gathers them into `recipes.json`, and `index.html` displays them with search and scaling. Pages CMS gives you a form to add and edit recipes.

## One-time setup

1. **Create a repo.** On github.com, make a new repository (e.g. `recipes`). Free GitHub Pages needs the repo to be public, so anyone with the link can see the recipes. A private repo with Pages needs a paid plan.
2. **Upload the files.** In the new repo, choose "uploading an existing file" and drag in everything from this folder, including the `_recipes` folder. Commit.
   - `.pages.yml` starts with a dot, so your computer may hide it (on a Mac, press Cmd+Shift+. in Finder to show it). If it doesn't upload, use "Add file > Create new file", name it `.pages.yml`, and paste its contents.
3. **Turn on Pages.** Repo Settings > Pages > Source: "Deploy from a branch", branch `main`, folder `/ (root)`. Save. After a minute or two the site is live at `https://<your-username>.github.io/recipes/`.
4. **Connect Pages CMS.** Go to https://app.pagescms.org, sign in with GitHub, give it access to the `recipes` repo, and open it. You'll see "Recipes" with a form for each one. Bookmark it on your phone.

## Day to day

- **Add or edit:** use Pages CMS. Saving commits the file, and the site updates about a minute later.
- **Quantities** are numbers only (decimals OK). Put the unit in the unit field.
- **Steps** are one entry per step. **Notes** is optional free text.
- **Every change is in the repo history**, so you can always get an old version back.

## Using the site

- Search matches recipe names and ingredients.
- Scale with ½×, 1×, 2×, a custom factor, or tap any quantity and type the amount you have (e.g. 100 g of egg whites) to scale everything to it.
- Tap a step to check it off.
- "Keep screen on" stops your phone from sleeping while you cook (supported browsers only).

## Files

- `_recipes/*.md`: the recipes (YAML between the `---` lines)
- `index.html`: the viewer page
- `recipes.json`: template that builds the recipe list on GitHub
- `_config.yml`: GitHub Pages settings
- `.pages.yml`: Pages CMS form definition
