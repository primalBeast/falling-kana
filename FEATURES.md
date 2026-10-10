# Falling Kana — security-and-features branch

## Code review summary (client-side single-file game)

**Security posture:** Good for a pure client-side app.
- No server, no cookies, no eval, no innerHTML of user input.
- Input restricted to letters / Enter / Backspace / Space.
- localStorage only stores settings + high score, wrapped in try/catch.
- Added Content-Security-Policy meta tag.

**Remaining notes:** Google Fonts is an external load (privacy). No other remote code.

## Implemented on this branch
1. High score persistence (localStorage)
2. Pause / resume with Spacebar
3. Auto-pause when the tab loses focus
4. Best score shown in the HUD
5. Content-Security-Policy

## Additional useful features ready to layer
6. Simple Web Audio sound effects (success / miss / pause)
7. Practice focus mode (vowels, k-line, s-line, etc.)
8. Session timer and accuracy trend
9. Color theme selector (blue / green / purple)
10. Keyboard shortcut help overlay (press H)
11. Export / import settings as JSON
12. Combo streak visual badge
13. Mobile-friendly larger tap targets for menu
14. Daily challenge seed (same kana order for the day)
15. Optional romaji hint delay for Kanji

Branch: `security-and-features`
Play by opening index.html from this branch or enabling GitHub Pages.
