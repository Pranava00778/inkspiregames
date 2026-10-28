# Inkspire Ink Drop

A one-page game for the Delhi Horror Con flyer. Catch the dripping ink in the pot to unlock a stall discount code.

Everything lives in `index.html` (HTML, CSS and JS in one file). There is no build step.

## Change the game

Open `index.html` and edit the `CFG` block at the top of the script:

- `goal`: drops needed to fill the pot
- `maxSpills`: drops a player can spill before losing
- `prefix`: start of every discount code
- `offer`: the line shown under the code

## Test it

- Open `index.html` in a browser, or run `npx serve .` in this folder.
- Each phone gets one try and one code, stored in the browser.
- Add `#reset` to the end of the address and reload to clear it on your own device.

## Deploy on Netlify

Drag and drop: go to https://app.netlify.com/drop and drop this whole folder.

Or from Git: push this folder to a GitHub repo, then in Netlify choose Add new site, Import an existing project, pick the repo. Leave the build command empty and set the publish directory to `.` (already set in `netlify.toml`). Every push to the main branch redeploys.

After the first deploy, point the flyer's QR code at the Netlify address. Set a custom site name under Site configuration, Change site name, before you print so the link stays short and fixed.
