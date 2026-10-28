# BrewHouse

A website for a fictional specialty coffee shop: homepage, interactive menu (20 items, INR prices), drink customisation, cart, simulated pickup ordering, About and Contact.

**Orders are simulated.** Nothing is sent to a server, no payment is taken, and no real café receives anything. The site says so on every page, in the cart, at checkout and on the confirmation.

Plain HTML, CSS and JavaScript. No build step, backend or API keys. The cart is saved in the browser's localStorage.

## Files

- `index.html` page structure
- `styles.css` design
- `menu.js` menu items, prices and categories (edit here)
- `app.js` menu filters, search, cart, checkout

## Run locally

Open `index.html` in a browser, or run `npx serve .` in this folder.

## Using real photos

Menu cards use built-in illustrations. To use photos, put images in an `images/` folder and add a field to an item in `menu.js`, for example `photo: 'images/flat-white.jpg'`.

## Deploy with GitHub and Netlify

1. Create a new empty repository on GitHub.
2. In this folder run:
   ```
   git init
   git add .
   git commit -m "BrewHouse website"
   git branch -M main
   git remote add origin https://github.com/YOUR-USERNAME/brewhouse.git
   git push -u origin main
   ```
3. In Netlify choose Add new site, then Import an existing project, and pick the GitHub repository.
4. Leave the build command empty and set the publish directory to `/` (the repository root). Click Deploy.

No GitHub? Drag this folder onto https://app.netlify.com/drop instead.

To use GitHub Pages instead: repository Settings, Pages, deploy from the `main` branch root.
