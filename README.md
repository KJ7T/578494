# [NODE NUMBER] Node Page — Starter Kit

*Starter Kit version 1.1 (September 19, 2026)*

Off-node reference site for an AllStarLink node, built with GitHub Pages
using Jekyll's `minima` theme. GitHub builds this automatically from the
Markdown files on push — there is no local build or deploy step.

## Before you push this anywhere

Every file in this kit has bracketed placeholders like `578494` and
`KJ7T` — find and replace them with your own information before
publishing. `about.md`, `disclaimers.md`, and `changelog.md` also have
italicized instructional text describing what belongs in each section;
replace that with your own real content.

## Structure

- `_config.yml` — site settings and theme
- `index.md` — home page
- `about.md`, `disclaimers.md`, `changelog.md` — content pages, linked
  from the home page and the site nav
- `_includes/node-status.html` — the live Online/Offline indicator shown
  on the home page (new in version 1.1)

See the full how-to guide this kit accompanies for setup instructions.

## What's new in version 1.1

The home page now shows a live Online / Offline / Status unavailable
indicator, with a "Check now" button. It reads AllStarLink's public
statistics for your node in the visitor's browser; it does not ping your
node. The indicator is added by one `include` line in `index.md`, and it
picks up your node number when you replace `[NODE NUMBER]` in that file
like everything else. To remove it, open `index.md`, delete the comment
block and the `include` line under the intro paragraph, and delete the
`_includes` folder. The guide has a section that explains the indicator
and how to adjust it.
