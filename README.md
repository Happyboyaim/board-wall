# Board Wall

A full-screen collage of Pinterest pins that drifts slowly upward, made to run on an iPad like a screensaver.

## What's in this folder

- `index.html`: the whole app (collage, status bar, Boards screen).
- `manifest.webmanifest`, `icon-180.png`, `icon-512.png`: let it open full screen from the iPad Home Screen with its own icon.

## How it gets pins

The iPad reads each board from Pinterest's public board widget feed (the same feed Pinterest's embeddable board widget uses). Boards must be public. Secret boards and board sections don't work. If no board can be read, the page shows the last pins it read successfully, and otherwise sample images, and the status bar says so.

## Put it online (GitHub Pages, free)

1. On github.com, create a new public repository, for example `board-wall`.
2. Upload these files to it (Add file > Upload files), then commit.
3. In the repository: Settings > Pages > Build and deployment > Source: Deploy from a branch. Branch: `main`, folder `/ (root)`. Save.
4. After a minute or two the page is at `https://YOUR-GITHUB-NAME.github.io/board-wall/`.

## Set it up on the iPad

1. Open that address in Safari.
2. Tap Share > Add to Home Screen. Keep "Open as Web App" on, then tap Add.
3. Open Board Wall from the Home Screen. Tap anywhere, then Boards, to save boards and pick which ones show. The Home Screen app keeps its own saved boards, separate from Safari.
4. Keep the screen on: Settings > Display & Brightness > Auto-Lock > Never. Leave the iPad plugged in.
5. Optional, to stop the app being swiped away: Settings > Accessibility > Guided Access > on, set a passcode, and set Display Auto-Lock to Never. Open Board Wall, triple-click the top button, tap Start. Triple-click again and enter the passcode to end.

## Saved boards

Tap the wall > Boards. Every board you save stays in the list.
- **Save a board:** paste its link (and an optional name), tap Save board.
- **Switch to one board:** tap Show next to it.
- **Mix boards:** tick several, then tap Show ticked boards.
- **Remove:** tap Remove, then Show ticked boards to keep the change.

You can also open the address with `?boards=` and comma-separated links, for example `?boards=pinterest.com/dankong2004/2027,pinterest.com/dankong2004/another-board`.

Boards are re-read every 6 hours while the app is open. Nothing appears on screen unless you tap, or a board can't be read.
