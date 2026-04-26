# 🌐 Muazz — Portfolio

> Hand-written HTML/CSS/JS. No framework. No `node_modules`.
> No analytics tracking your scroll depth.
>
> Just a portfolio.

```
$ ls -la
drwxr-xr-x  Images/        site-wide imagery
drwxr-xr-x  Lately/        what I've been making/reading lately
drwxr-xr-x  Projects/      smaller things, screenshots, demos
drwxr-xr-x  Side Quests/   the fun stuff — talks, events, oddities
drwxr-xr-x  Work/          source assets for case studies
-rw-r--r--  index.html     home page
-rw-r--r--  *.html         case study pages, one per role
-rw-r--r--  copy.md        living doc of every word on the site

$ wc -l index.html
   ~2000 lines of love-it-or-hate-it vanilla HTML/CSS/JS
```

## Why static? Why no framework?

⚡ **It's fast.** Cold load is one HTTP round-trip for the HTML, then
parallel image fetches. No JS framework hydration tax. No critical
CSS extraction. No bundle size to optimize.

📦 **It's portable.** Works on GitHub Pages, Cloudflare Pages,
Netlify, S3, my friend's Raspberry Pi, a thumb drive.

🛡️ **It outlasts me.** I've watched three personal sites die because
their build pipeline broke after a Node version bump.
This one is six files and a folder. **No toolchain decay.**

📱 **It's editable from anywhere.** I've added paragraphs from my
phone using GitHub's web editor. From an airport. While bored.

## Local dev

```bash
# any static server works
python3 -m http.server 8000

# or
npx serve .

# or just double-click index.html
```

Yeah, that's it.

## Stack (such as it is)

- **HTML** (lots of it)
- **CSS** (vanilla — no Tailwind, no preprocessor, no PostCSS)
- **JS** (very little of it, no framework, no jQuery)
- A bit of **SVG** for diagrams and logos

That's the entire stack. There's no `package.json`. There's no
build step.

## Deploying

```bash
git push origin main
# (the site is published from this branch)
```

That's the deploy story. No CI. No preview environments. No
`vercel.json`.

## On the to-do list

- 🌙 A real dark mode that isn't just `prefers-color-scheme`
- 📱 Better mobile case-study layout (the desktop grid isn't
  vertical-scroll friendly)
- 🗂️ An index of "lately" entries so the page doesn't grow forever
- 🔗 Permalinks for individual lately entries

## Why hand-write a portfolio in 2026?

Because every PM-portfolio template ends up looking the same —
neutral type, big hero image, three-column "Selected Work" grid,
identical CTA at the bottom.

Hand-rolling lets me put **the weird, specific, slightly-off thing**
exactly where I want it. The case study photo with the wrong border
radius because I liked it that way. The font at 18px instead of the
"correct" 16px. The opinion that doesn't fit a template.

Also, the constraint of *"no framework"* is its own creative prompt.
Every CSS animation has to be hand-coded. Every interaction is a
DOM event listener. It keeps the website honest.

Try it sometime.

---

*Built without `npm install`. Maintained one paragraph at a time.*
