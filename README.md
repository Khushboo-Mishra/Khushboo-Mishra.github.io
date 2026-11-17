# Khushboo Mishra, portfolio

Static site. One `index.html` plus a `media/` folder of GIFs, no build step, no dependencies. Fonts load from Google Fonts and fall back to system fonts.

## Publish on GitHub Pages

The repo must be named exactly `Khushboo-Mishra.github.io` to get the address `https://khushboo-mishra.github.io/`.

1. On GitHub, create a new **public** repo named `Khushboo-Mishra.github.io` (empty, no README).
2. From the folder containing these files:

   ```bash
   git init -b main
   git add .
   git commit -m "Add portfolio site"
   git remote add origin https://github.com/Khushboo-Mishra/Khushboo-Mishra.github.io.git
   git push -u origin main
   ```

3. In the repo, open **Settings > Pages**. Under **Build and deployment**, set Source to **Deploy from a branch**, branch `main`, folder `/ (root)`. Save.
4. After about a minute the site is live at `https://khushboo-mishra.github.io/`.

Your SQL-MCP-101 tutorial already lives at `/SQL-MCP-101/` on the same domain, and this site does not touch it.

## Editing

Everything is in `index.html`. Search for the section ids: `work`, `wins`, `experience`, `skills`, `contact`.
The "Last pushed" dates on the project cards are fetched live from the GitHub API and disappear quietly if the request fails.

## Media

`media/*.gif` are screen recordings of your own project pages (Creator Matchmaker, AgentOps, SQL-MCP-101). The matching `.png` files are static posters that visitors with "reduce motion" turned on see instead. Keep the `media/` folder when you commit.
