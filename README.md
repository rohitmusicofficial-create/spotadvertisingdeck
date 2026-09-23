# Spot Advertising — animated corporate profile

A single-page animated deck. No build step, no dependencies, no framework.
Two files do everything: `index.html` and `vercel.json`.

---

## Deploy to Vercel, the drag-and-drop way (easiest, about 2 minutes)

1. Download the `spot-deck` folder so you have `index.html`, `vercel.json` and this
   README sitting together in one folder on your machine.
2. Go to **vercel.com** and sign in. A free Hobby account is enough.
3. On the dashboard, click **Add New** and then **Project**.
4. Look for the **deploy a template or drag a folder** option on that screen, and
   drag the whole `spot-deck` folder into the drop area. Drag the folder itself,
   not the files inside it.
5. Vercel detects it as a static site automatically. Leave every setting as it is.
   Do not pick a framework. Do not set a build command.
6. Click **Deploy** and wait. It takes under a minute.
7. You get a live URL that looks like `spot-deck-xxxx.vercel.app`. That link is
   shareable immediately.

## Deploy from GitHub instead (better if you will keep editing it)

1. Create a new repository on GitHub and upload these files to it.
2. On Vercel, click **Add New**, then **Project**, then **Import Git Repository**.
3. Pick the repo. Framework preset: **Other**. Leave build command and output
   directory empty.
4. Click **Deploy**.

Every time you push a change to GitHub, Vercel redeploys on its own.

## Putting it on a real domain

1. Open the project on Vercel and go to **Settings**, then **Domains**.
2. Add the domain, for example `profile.spotadvertising.in`.
3. Vercel shows you the DNS record to add. Add that record wherever the domain is
   registered. It usually goes live within the hour.

---

## Presenting it

- **Arrow keys**, **Page Up / Page Down** or **Space** move one slide at a time.
- **Home** and **End** jump to the start and the finish.
- The **dots on the right edge** are clickable, so you can jump straight to a
  section if a client asks about one.
- Scrolling snaps section to section, so it never stops halfway between two slides.
- Press **F11** (Windows) or **Control + Command + F** (Mac) for full screen before
  you present.

## What animates on its own

- The out-of-home board cycles through all six advertiser frames on a live ten
  second countdown ring. This runs only while that slide is on screen.
- The live campaign monitor keeps ticking upward the whole time it is visible.
- Counters, the metro line, the seat grid and the funnel all animate on arrival.

## Editing the content

Everything is in `index.html`. The text lives in two places:

- Headlines and paragraphs sit in the HTML, inside each `<section>`.
- Repeating items (client names, service columns, funnel steps, dashboard numbers)
  sit in the script at the bottom, in plain lists near the top of it. Each list is
  labelled with a comment such as `/* clients */` or `/* funnel nodes */`.

Change the words inside the quote marks and save. Nothing else needs touching.

## Honesty note worth keeping

The funnel numbers on the measurement slide and everything in the campaign monitor
are **sample values**, and both slides say so on screen. Replace them with real
campaign data before showing this to a client who might reasonably read them as
their own account.
