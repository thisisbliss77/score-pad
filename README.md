# Score Pad

Score Pad is a score keeper for card, dice and board games. It runs in any modern browser on a phone, tablet or computer, needs no account and no install, and keeps working offline once it has been opened.

## What it does

Score Pad comes with ready-made score sheets for 23 games, and you can make your own for anything else.

- **Built-in games:** Hearts, Spades, Euchre, Pinochle, Oh Hell, Wizard, Gin Rummy, Rummy 500, Canasta, Phase 10, Five Crowns, Cribbage, Uno, Golf, Lost Cities, Yahtzee, Farkle, Scrabble, Mexican Train, Biriba, Xeri, Diloti and Tavli.
- **Custom games:** name a game, add players, and add extra columns for bids, tricks or bonuses. Save any setup as a template to reuse it.
- **Scoring help:** running totals, a dealer marker that rotates each round, pre-filled boards for games with a fixed number of rounds, automatic scoring for Lost Cities and the Yahtzee upper bonus, and entry limits taken from each game's rules.
- **Rules:** a Rules button on every built-in game with Setup, Deal, Play, Scoring and Winning tabs.
- **History and leaderboard:** finished games are kept with their end date, and a leaderboard ranks players by wins across all games or one game.
- **Import and export:** move your games and templates to another device as a file or as text.

## Put it online with GitHub Pages

You need a free GitHub account. The site will be public, so anyone with the link can use it.

1. Create a new **public** repository on GitHub, for example `score-pad`.
2. Unzip the download. On the repository page choose **Add file**, then **Upload files**, and drag in everything inside the folder: `index.html`, `sw.js`, `manifest.webmanifest`, `icon.svg`, the three `.png` icons, `.nojekyll` and this `README.md`. Commit the upload.
3. Open the repository's **Settings**, then **Pages** in the sidebar.
4. Under **Build and deployment**, set **Source** to **Deploy from a branch**.
5. Choose the `main` branch and the `/ (root)` folder, then click **Save**.
6. After a minute or two, the Pages screen shows the address of your site. It normally looks like `https://YOUR-USERNAME.github.io/score-pad/`.

Share that address with anyone you want to use Score Pad.

## Using it like an app

Open the address on a phone and add it to the home screen. On iPhone, use the Share button in Safari and choose **Add to Home Screen**. On Android, use the browser menu and choose **Add to Home screen** or **Install app**. It then opens full screen with its own icon and works without a connection.

## Where the data lives

Each person's games are saved in their own browser on their own device. Nothing is sent to a server, and nobody else can see anyone's scores.

This has three consequences worth knowing:

- Two phones do not share a live game. One person keeps score, or each keeps their own.
- Clearing the browser's site data, or using a private window, removes the saved games.
- To move games to another device, use **Export** on the old one and **Import** on the new one.

## Updating the app

Replace `index.html` in the repository with the new version. Then open `sw.js` and change `score-pad-v1` to `score-pad-v2` (and so on each time), so phones that already have the app pick up the new version instead of the saved copy.

## Files

| File | Purpose |
|---|---|
| `index.html` | The whole app: page, styles and code in one file |
| `sw.js` | Lets the app work offline |
| `manifest.webmanifest` | Name, colors and icons for the home-screen app |
| `icon.svg`, `icon-192.png`, `icon-512.png`, `apple-touch-icon.png` | App icons |
| `.nojekyll` | Tells GitHub Pages to serve the files as they are |

The app loads its two typefaces (Inter and Space Grotesk) from Google Fonts. Without a connection it falls back to the device's own fonts.

## Rules and scoring

The rules summaries are written in our own words and were checked against published sources, mainly Pagat's card game rules and the publishers' instruction sheets where those were available. House rules vary, so treat the Rules tabs as a reminder rather than a ruling. Custom games have no limits or rules attached.

## Names and trademarks

Score Pad is an independent score-keeping tool. It is not affiliated with, endorsed by or sponsored by the publisher of any game. Game names such as Uno, Phase 10, Yahtzee, Scrabble, Wizard, Five Crowns and Lost Cities are trademarks of their respective owners and are used here only to say which game a score sheet is for. The icons are original drawings, not the publishers' logos.

## License

No license file is included. If you want others to be free to copy or change the code, add a license of your choice to the repository, for example through GitHub's **Add file** and **Create new file** flow, which offers license templates when you name the file `LICENSE`.
