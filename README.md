# calm-ink — a QLMarkdown theme

A quiet markdown QuickLook theme for macOS, faithful to the [calm](https://github.com/shakilclark/calm) identity: monochrome ink on paper, the locked typefaces, hierarchy carried by space and weight rather than colour. Built for [QLMarkdown](https://github.com/sbarex/QLMarkdown).

## The look

- **Ink on paper, both modes.** Warm off-white paper with near-black ink in light; soft off-black with bone-white ink in dark — never screen-white, so it reads as paper. Values are calm's locked tokens.
- **Type does the work.** Atkinson Hyperlegible for body, Yrsa for headings, IBM Plex Mono for code — the calm quartet, with a generous line-height and a comfortable reading measure.
- **Code is quiet.** Syntax colour-coding is off; a reader is a reading surface, not a working terminal, so code differentiates by weight, not hue.
- **One soft accent.** Links sit in calm's clay, softly underlined — visible, never loud. The same clay is the one whisper on a blockquote's edge.

## Install

1. Install QLMarkdown: `brew install --cask qlmarkdown`
2. Install the typefaces (skip any you have):
   ```
   brew install --cask font-atkinson-hyperlegible font-yrsa font-ibm-plex-mono
   ```
3. Copy `calm-ink.css` into QLMarkdown's styles folder:
   ```
   ~/Library/Group Containers/group.org.sbarex.qlmarkdown/Library/Application Support/styles/
   ```
4. Open **QLMarkdown → Preferences**, set **Theme → calm-ink** (leave the mode on *Extend default*), **Appearance → Auto**, then **⌘S** (or turn on *Autosave settings*).
5. Select any `.md` in Finder and press **space**.

## Notes

- The style *extends* QLMarkdown's default theme — it remaps the base CSS variables to calm's palette and overrides the typefaces, so it rides the existing structure rather than replacing it.
- Colour values and typeface choices come straight from calm's [`tokens.css`](https://github.com/shakilclark/calm/blob/main/tokens.css) and [`docs/identity.md`](https://github.com/shakilclark/calm/blob/main/docs/identity.md) — change is by deliberate revision, not drift.
