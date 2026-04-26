# Muazz — Portfolio

The site at `index.html`. Hand-written HTML/CSS/JS. No frameworks,
no build step, no `node_modules`, no analytics tracking your scroll
depth.

Just a portfolio.

## What's inside

```
index.html         Home — short bio, work, side projects, "lately"
*.html             Case study pages (one per substantial role)
Projects/          Smaller things, screenshots, embedded demos
Side Quests/       The fun stuff — community events, talks, oddities
Lately/            What I've been making/reading/thinking recently
Work/              Source assets for case studies (logos, screenshots)
Images/            Site-wide imagery
copy.md            Living doc of all the words on the site
```

## Why static

- **It's fast.** Cold load is one HTTP round-trip for the HTML, then
  parallel images. No JS framework hydration tax.
- **It's portable.** Works on GitHub Pages, Cloudflare Pages, Netlify,
  S3, my friend's Raspberry Pi.
- **It outlasts me.** I've watched three personal sites die because
  their build pipeline broke. This one is six files and a folder —
  no toolchain decay.
- **It's editable from anywhere.** I've added paragraphs from my
  phone using GitHub's web editor at airports.

## Local dev

```bash
# any static server works
python3 -m http.server 8000
# or
npx serve .
# or just double-click index.html
```

## Stack (such as it is)

- HTML
- CSS (vanilla, no Tailwind, no preprocessor)
- JS (vanilla, very little of it)
- A bit of SVG for diagrams and logos

That's it.

## Deploying

Push to `main`. The site is published from this branch.

## Things on the to-do list

- A dark mode that isn't just `prefers-color-scheme`
- Better mobile case-study layout (the desktop-grid isn't friendly
  to vertical scrolling)
- An index of "lately" entries so the page doesn't grow forever

## Why hand-write a portfolio in 2026?

Because every PM-portfolio template ends up looking the same —
neutral type, big hero image, three-column "Selected Work" grid.
Hand-rolling lets me put the weird, specific, slightly-off thing
exactly where I want it.

Also, the constraint of "no framework" is its own creative prompt.
Try it sometime.
