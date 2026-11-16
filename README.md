# getcmdigital.com

The CM Digital website. One self-contained `index.html` — no build step, no
dependencies, no framework.

## How it goes live

This repo is linked to the Netlify project `helpful-bonbon-73c3ed`
(getcmdigital.com). **Anything pushed to `main` deploys automatically**,
usually within a minute. There is nothing to run locally and nothing to build.

## Files

| File | What it is |
| --- | --- |
| `index.html` | The entire site: markup, styles, scripts, and the four example demos |
| `netlify.toml` | Tells Netlify to publish this folder as-is and not to cache index.html |

## Assets that aren't here yet

`chris.jpg` (founder photo) and `ai-demo.mp3` (sample call) are referenced by
the page but not in the repo. The page is built to handle their absence: the
photo slot falls back to a "CM" badge and the audio player stays hidden. Drop
either file in the root and it appears on the next deploy.

## Forms

The contact form posts to Netlify Forms under the name `contact`. Both the
short form near the top of the page and the long one at the bottom submit to
that same form, so every lead lands in one place:
Netlify → Project → Forms → contact.

## Editing

It's one file. Open it, change it, commit, push. Claude can do this directly
once the repo is attached to a session.
