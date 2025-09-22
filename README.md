# Presentations

Static presentation site powered by [reveal.js](https://revealjs.com/) and GitHub Pages.

## Repo layout
- `index.html` – bootstraps Reveal and loads slides from `slides.md`.
- `slides.md` – sample deck content written in Markdown.
- `reveal.js/` – upstream Reveal.js clone that provides assets and plugins.

## Local preview
1. Ensure Python 3 is installed.
2. From the repo root run `python3 -m http.server 8080`.
3. Open `http://localhost:8080` in a browser to view the deck.

## Publishing to GitHub Pages
1. Create a new GitHub repository named `presentations` and push this project to the `main` branch.
2. In the GitHub repo, open **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from branch**.
4. Select `main` as the branch and `/ (root)` as the folder, then click **Save**.
5. After GitHub finishes the build, your deck will be live at `https://<username>.github.io/presentations/`.

## Customising the deck
- Edit `slides.md` to add or reorder slides. Horizontal sections use `---`, vertical stacks use `------`.
- Update the theme by changing the stylesheet import in `index.html` (e.g. `dist/theme/league.css`).
- Add plugins by updating the `<script>` tags at the bottom of `index.html` and enabling them in `Reveal.initialize`.

## Keeping Reveal.js updated
Run `git -C reveal.js pull` to fetch the latest upstream changes. Commit the updated files to your repository when ready.

## Additional decks
- [`diss-induction/`](diss-induction/) – Year 3 BSc Psychology project induction deck.
